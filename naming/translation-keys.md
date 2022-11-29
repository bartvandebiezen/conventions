# Translation Keys

## Write keys in US English

## Prefer hyphens as delimiters or use camelCase

When hyphens are not possible because of specific code language or framework use camelCase.

## Categorize keys with name of component, page, screen or flow

- Make sure the name of category is well thought before categorizing keys.

Examples:

- notifications.idle-message-text -> Your session has expired because you were longer than %time% inactive. Please renew your selection.
- login.current-password-label -> Your password

## Categorize keys used in different components or pages in ‘global’

Examples:

- global.edit-action -> Edit
- global.optional-lowercase -> optional

## Keys containing ‘exact translations’ should contain only the exact words and end with the type of capitalization

The descriptions for capitalization is borrowed from CSS’s text-transform. Although CSS text-transform does not follow language-specific casing, this should of course be the case in the translations.

Examples:

- global.monday-capitalize -> Monday
- global.monday-lowercase -> monday
- global.monday-uppercase -> MONDAY

## Keys which are a abbreviations end with ‘short’

Capitalization type is added after the term ‘short’.

Examples:

- global.friday-short-capitalize -> Fr.

## Keys for a title end with ‘title’

The term ‘title’ gives important information about its context and how it should be translated. It is also language-specific, for example: in Dutch, only the first character is capitalized; in English, all the main words are capitalized (i.e. title casing).

Examples:

- login.login-page.title -> Login
- checkout.payment-method-page.title -> Payment Method
- checkout.payment-failed-page.title -> Payment was Unsuccessful

## Keys for longer texts end with ‘text’

Examples:

- checkout.payment-failed-page.text -> Try again or change payment method.

## Keys for HTML content should end with 'rich-text'

Examples:

- checkout.payment-failed-page.rich-text -> `<p>Try again or change payment method.</p>`

## Keys for form labels end with ‘label’

Short description of what is expected from the user to fill in. These keys do not only contain labels that can be found in front of input fields, they can also contain labels found after radio buttons and checkboxes or in segmented controls.

Examples:

- checkout.personal-information-page.mister-short-label -> Mr.
- checkout.personal-information-page.email-label -> Email

## Keys for ‘form helper texts’ end with ‘helper-text’

Helper text are always visible directly below an input field. It helps the user to know what is expected and why it is needed.

Examples:

- checkout.personal-information-page.email-helper-text -> You will receive a confirmation by email.

## Keys for ‘form feedback texts’ end with ‘feedback-text’

Feedback text gives feedback about why the data within an input field is incorrect and how the user can solve this. Feedback text is only visible after the user gets an error when submitting a form.

Examples:

- checkout.personal-information-page.email-empty-feedback-text -> Your email address is needed to finish your booking.

## Keys for file names end with ‘file-name’

File names should not include the format of the document. This should be added by the back-end.

Examples:
- global.general-conditions-file-name -> general-conditions

## Keys for buttons, links or actions end with action

Examples:
- global.close-action -> Close

### Use imperative for direct actions
The key in a button that directly performs the desired action must be written imperative. So 'Save' instead of 'To save'. In English, this is often done correctly, but for instance in Dutch these are often mixed up. In Dutch write 'Bewaar' instead of 'Bewaren'.

Examples:
- global.save-action -> Bewaar

### Use infinitive or imperative for indirect actions depending on language
A button or link that refers to a page or form in which the action can be performed, must be written:
- Infinitive in Dutch: write 'Reserveren' instead of 'Reserveer' for the reference to the reservation form. Titles of a form must also be written infinitive, so the title of the login form has the title 'Inloggen' and not 'Log in'.
- Imperative in English: the same as direct actions.

Examples:
- global.to-save-action -> Bewaren

### Ellipsis to indicate folow-up actions should not be part of the translation
If an action has follow-up actions to complete it, it should end with an ellipsis. An ellipsis should not be part of the translation. It should be added by a developer to the codebase immediately after the translation key. This gives flexibility to replace an ellipse with, for example, a chevron without having to change the content or translation key.
