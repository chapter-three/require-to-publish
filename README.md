Require-to-publish
==================

A Drupal module which allows required fields to remain empty as long as the node is unpublished. Also, it creates a "Save as Draft" button.

There is a D6 module which does this already: https://drupal.org/project/required_for_pub

This module does more than just create a "Save as Draft" button. 

It allows any field to be configured as "required for content to be published." When entering data on the node add or edit form, 
user will see "*Required for content to be published" right below the field label.

Moreover, when a user tries to publish the content without entering data for fields that are "required for content to be published",
2 things are triggered: 
1. An error message stating the fields that require data, and 
2. the field itself will be "highlighted" in red, 
behaving much like the Drupal core's red highlight for fields configured to be "required."

Example use cases:
==================

1. A donation cannot be submitted (or published ) until the donation amount is selected from  1 of say, 3 choices ($100, $50, or $10).

2. A Review on a article cannot be submitted unless a grade or rating is given (A, B, C, D , F  OR 5 stars, 4 stars or 3 stars)

When no field has been configured for the entire node, the "Save as Draft" button will not display.

Roadmap: 

Try to make compatible with Workbench, which handles status per revision rather than per node. Allow Workbench to set "require" level to an arbitrary state? (For instance, not required for "Draft" but required for "Needs Review" or "Published"?)
