# Making HTML templates editable
### Blocks Edit's library of tags to define editable features in your email template

**The Blocks Edit CMS framework is a simple library of tags based on classes, styles, and attributes that you add to your HTML code to define editable features.** It follows [modular design](https://blocksedit.com/email-template-guide/) practices and standard [production systems](https://blocksedit.com/email-design-system/) so it works around your email template code.

See also: [Considerations for setting up your template](https://blocksedit.com/developer/getting-started/) | [Example template code](https://blocksedit.com/developer/editable-email/)

- **Content:** Pieces of text, images, and links [View tags →](https://blocksedit.com/developer/content/)

- **Components** Stand-alone functional elements [View tags →](https://blocksedit.com/developer/components/)

- **Regions:** Customizable areas that can't be moved around [View tags →](https://blocksedit.com/developer/regions/)

- **Sections:** Stackable containers for layout options [View tags →](https://blocksedit.com/developer/sections/)

- **Groups:** Design variations of areas to choose from [View tags →](https://blocksedit.com/developer/groups/)

## Working with your template

### Importing to test results
You can try out the editable features that you've added tags in your code for by just importing your HTML file into Blocks Edit. Log in to your account ([sign up for free](https://app.blocksedit.com/signup/)) and click the "Import template" option at the top of your dashboard.

### Preview mode
Try out a template's features after import without having to create emails. Click on the title of your template from the dashboard to go into preview mode. Any edits you make here are not saved. However, you can save layouts to be reused in emails.

### Template versions
While in preview mode, you can also update a current template by uploading a new version of it using the "Import new version" option at the top. New emails will be created based on the latest version. Any emails created from previous versions will continue to work, but with features only from the specific version each email was created from.

## Additional dev features

### Quick adjustments using browser dev tools
While in edit mode for an email, you can use your browser's dev tools to make edits to your HTML and then click the "Save" button to actually save the updated code! Using this option should be limited to fixes, tweaks, or minor HTML and CSS changes to a particular email. Changes will only be saved to that email. We don't recommend adding any Blocks Edit editable tags. You will also see Blocks Edit UI in the code that you'll have to avoid.

### Hiding content
If you want to hide certain areas from being seen in Blocks Edit when working with an email, wrap your code with the 'block-hide' option.

```
<!-- block-hide -->
<p>Content</p>
<!-- end-block-hide -->
```

### Email portions
You can import just a portion of an email for editing. This may be helpful if you have a current email provider that uses a master template and locks in the header and footer for example, and you just want to work with a particular module. Or, if you want to provide your team with templated email signatures to use.

## Updates log
- **9/29/2019:** Adds ability to hide certain code from displaying in the editor
- **9/6/2019:** Adds <code>block-preview</code> class for preview text
- **8/22/2019:** Changes <code>data-style</code> attribute and <code>-style-var</code> style to <code>data-group</code> and <code>-group-var</code>, respectively
- **8/7/2019:** Allows for HTML snippets to be imported without requiring head/body/html tags
- **11/29/2018:** Adds <code>block-background</code> class and <code>-block-background: true</code> style for background image editing
- **8/25/2018:** Allows regions to enable showing border only with no options
- **2/20/2018:** Adds alternate versions functionality to sections
- **12/18/2017:** Adds <code>data-block="variable-name"</code> attribute and <code>-block-var: 'variable-name'</code> style for storing content
- **11/30/2017:** Adds <code>block-component</code> class and <code>-block-component: true</code> style for stand-alone components functionality
- **11/30/2017:** Adds <code>data-style="variable-name"</code> attribute and <code>-style-var: 'variable-name'</code> style for alternate region versions
- **11/30/2017:** Adds <code>block-section</code> class and <code>-block-section: true</code> style for stackabe sections to drag in to add
