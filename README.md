# LWC_contactCreator

=>in the contactCreator.html
Line 3: By using lightning-record-form in the markup, we get all of the security and performance benefits that Lightning Data Service provides. When lightning-record-form doesn’t specify a recordId, it operates in edit mode, and creates a record on submit.
Line 4: Binding the object-api-name property indicates the kind of object to load.
Line 5: Binding the fields property indicates the fields to show in the form.
Line 6: We set handleSuccess as the handler for the success event.


=>in contactCreator.Js
Lines 3–6: At the beginning of the file, we import references to the Contact object and its fields. Referencing objects and fields in this way ensures referential integrity.
Salesforce verifies that the object and fields exist, prevents them from being deleted, and ensures that they are included in change sets and packages that 
reference the component. Importing object and field references ensures that your component code still works if the object or fields are renamed.

We define the handleSuccess event handler for the sucess event. handleSuccess is executed when the save operation succeeds. 
We show a toad message by firing ShowToastEvent, in which event.detail.di is a reference to the id propery of the newly created record.
