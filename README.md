Let's revisit Survey Gorilla, our Sinatra polling application.

Redo this application in Rails while practicing TDD. Focus on the models first and foremost. Write some integration tests to verify that the question adding/removing is working as you expect.

When creating a new survey, we'll be simultaneously creating a series of questions and possible choices. This will be your first introduction to nested form helpers using fields_for. Read the "Nested Attributes Example."

Objectives
Aside from practicing more TDD, nested forms and attributes are one of the last big moving pieces of Rails we haven't covered. Here is the documentation on ActiveRecord's nested attributes.

Nested attributes only have to do with ActiveRecord. Read and understand the linked examples — nested attributes allow you to create, update, and even destroy associated models in a single create call on the parent model.

Nested form helpers work by creating a form which results in a params hash arranged "just so" to take advantage of nested attributes. This way one can post a single form to a single action and create multiple database records in a single pass.