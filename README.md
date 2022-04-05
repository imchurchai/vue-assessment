## Setup

    npm install
    npm run serve

To show that everything is set up correctly, a simple UI is contained in `App.vue`, displaying a counter that is incremented when the accompanying button is clicked.

## Requirements
Create a contact management user interface in `App.vue`.

### Wireframe

    [ toolbar: add | edit | up | down ]
    [ table                    
      [ headers: (select) | Name | Phone ]
      [ contact rows: (select) | (name) | ( phone) ]
    ]

### A) UI:
1. Use Vuetify components to construct the UI consisting of a data table where contacts are listed, and a toolbar containing action buttons.
2. The data table should allow selecting a single contact in order for actions to be performed on the contact.
3. The `add` operation should show a dialog where the details for the new contact can be entered.
4. If all required inputs have been entered (name and phone), the dialog should allow the add operation to be completed.
5. The `edit` operation should show the same dialog to allow editing the selected contact.
6. The `up` operation should move the selected contact up one position in the list.
7. The `down` operation should move the selected contact down one position in the list.

### B) Store:
1. Maintain state for the list of contacts.
2. Provide a mutation for adding a new contact.
3. Provide a mutation for updating an existing contact.
4. Provide a mutation for moving a contact up one position in the list.
5. Provide a mutation for moving a contact down one position in the list.