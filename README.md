# Solid Data Playground

See the [data playground live on github pages](https://solid.github.io/form-playground/playground.html)

Play with solid forms. Apply a random form to a random object.

Todo: Create and edit forms, and associate forms with types.

## Basically how this works

You can accumulate  a set of resources you will need for the project. Drag them (their URIs))
into the big grey tray.

To save the project, put the URI of it into the top URI field.
 It should end with `/index.ttl#this`.  

You can apply various functions -- to be extended of course -- to one or two things on the web.

 - See the subject viewed with a given form
 - See a form viewed with the form form
 - See a SolidOD default view of the subject

## Experimental

 You can also set the subject URI for something new you want to create.
 Set the class of the new thing in the second URI field. Press the button.
You should be able then to edit details of the thing with the form of your choice.

You should be able to create a new form, in fact, and edit with with the form form.

Making a table view of some data, using a form to generate the query on
which the table is based.

## Possible future directions:

We need a form for editing SHACL shapes sop we can play with shapes in the same way.

 - Build simple apps using just a form or two: user level programming
 - Drill though to underlying shapes
 - Drill though to underlying ontology (schema)
 - Analyze, visualize ontologies
 - Collaboratively edit forms
 - Collaboratively edit shapes
 - Collaboratively edit ontologies
 - Collaboratively edit rules converting between different systems



## Simple data browser

There is also a webapp version of the data browser online: See
 [data browser webapp live on github pages](https://solid.github.io/form-playground/browse.html)

That is good if you want to point some linked data on the web at it as a general viewer.
It will also generate you a view URI for its view of that object for you to link to or show to others.
