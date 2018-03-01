## Questions

1. What does the second 'nil' argument in the line 6 text_field_tag of teachers/new.html.erb represent?
The 'nil' is like a default value for the form, so if you submit the form without any inputs for the course field, then it defaults to an empty string.

2. Go to `localhost:3000/teachers` in your browser; why does this not work?
This doesn't work because we haven't set up a route for the GET request yet.

3. What type of request did your browser just perform?
A GET request.

4. Go back to `localhost:3000/teachers/new`; submit the form again. What URL do you end up at?
We end up at localhost:3000/teachers.

5. Why does `localhost:3000/teachers` work now?
This works because we're now fetching data (from the form submission) and rendering it. In teachers_controller, we've defined a 'create' method in which we call "render 'show' ", which is associated with GET, so we're able to view the resulting HTML view.