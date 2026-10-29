---
name: save-contact
description: Save a person to ConnectMachine from what the user describes, with where and when they met. Use when the user mentions meeting someone or asks to save or add a contact.
---

# Save a contact

1. Pull out the name, company, job title, email, phone, where and when they met, and anything worth remembering. If the user didn't describe anyone, ask who they met.
2. Check whether the person already exists with `find_contact`. If one match comes back, offer to update that contact instead of creating a duplicate. If the result is ambiguous, ask which person they mean.
3. Create the contact with `create_contact`. Put where they met in `events` and the rest of the context in `notes`.
4. Confirm in one short line what was saved, and offer to add them to a network.

Don't invent details the user didn't give.
