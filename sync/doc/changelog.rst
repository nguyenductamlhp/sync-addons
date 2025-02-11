`13.0.1`
-------

- **Fix:** update params updating on existing records

`13.0.0`
-------

- **Fix:** Use `__sync.` for xmlid namespace to avoid data loss on module update.
- **Fix:** Use task ID in xmlid namespace for the task triggers.
- **Fix:** Keep job records (and their logs) on task deletion.
- **New:** Add *Sync Order* — advanced manual trigger with blackjack, partners list, text input, etc.
- **New:** Support `data.markdown` for custom documentation in the `DATA.🐫` tab.
- **New:** Add `MAGIC.group_by_lang` to eval context.
- **New:** Add dynamic Setting update via `PARAMS._update_param`.
- **New:** Add computed field `text` to the model `sync.data`. Usage example in dynamic code: `DATA.restaurant.text`.
- **Improvement:** Add `DATA.*` to the library eval context.
- **Improvement:** Update API for attaching dynamic values: `_set_sync_value`, `_get_sync_value`. No need to use `ir.property`.

`11.0.1`
-------

- **Improvement:** add `PARAMS.*` to the core eval context
- **Improvement:** clarify error message when model is not found

`11.0.0`
-------

- **New:** Use prime numbers for major releases ;-)
- **New:** Support data files
- **Fix:** Use Project ID for xmlid namespace
- **New:** Support dynamic properties
- **Improvement:** make links dependent on project

`7.0.0`
-------

- **New:** Dramatic improvement on Sync Studio API

`6.2.0`
-------

- **Improvement:** add method get_public_url() for attachment object


`6.1.0`
-------
- **Improvement:** use light telegram library in Telegram demo project (pyTelegramBotAPI)
- **Fix:** add button to show secret parameter value
- **Improvement:** add eval context function: `url2bin`
- **Fix:** Project export tool: add records of `sync.project.context`
- **Fix:** properly cleanup `base.automation` and action records

`6.0.1`
-------
- **Fix:** error on empty eval context in a project


`6.0.0`
-------

- **New:** support links with the same relation + refs, but different models
- **New:** projects can now use multiple execution contexts.

`5.1.1`
-------

- **Fix:** correct error message on link duplicates

`5.1.0`
-------

- **New:** add search filters for `sync.job` model

`5.0.2`
-------

- **Fix:** avoid base.automation errors after deleting sync.task
- **Improvement:** better names for triggers, Server Actions and Base Automation records

`5.0.1`
-------

- **Fix:** add missing `Trigger Fields` field in the Automation Trigger view

`5.0.0`
-------

- **Improvement:** run triggers with delay

`4.2.0`
-------

- **Improvement:** add eval context function `record2image`

`4.1.2`
-------

- **Improvement:** initial values do not overwrite parameter values after a module update.
- **Fix:** add exporting of text parameter values

`4.1.1`
-------

- **Fix:** For empty `links`, the property `links.odoo` must return empty recordset, not `None`

`4.1.0`
-------

- **Improvement:** add more eval context functions (`get_lang`, `url2base64`, `html2plaintext`)
- **Improvement:** add development tools (`LogExternalQuery`), add new type for `ir.logging`
- **Improvement:** move code checker above in task form to make it more visible
- **Fix:** delete `website_published` for sake of simplicity and to avoid webhooks problem on upgrading the module to v4.0.0+

`4.0.1`
-------

- **Fix:** set project as archived by default to avoid errors on installation and updating sync modules

`4.0.0`
-------

**Improvement:** remove Website module from dependencies, handle webhooks directly in Sync Studio

`3.1.2`
-------

- **Improvement:** Manager access group renamed to Administrator

`3.1.1`
-------

- **Fix:** allow getting link after setting it

`3.1.0`
-------

- **Improvement:** generate cleaner xmlid on generating XML data file
- **Improvement:** dynamically check python code for syntax errors
- **Fix:** support POST methods in http webhooks
- **Fix:** allow change field "active" for DB Triggers

`3.0.0`
-------

**Improvement:** add translatable multi-line parameters and make original params non-translatable
**Improvement:** add the possibility to fully duplicate the project

`2.1.3`
-------

- **Fix:** Export Xml: add missed field `filter_domain`, `filter_pre_domain`

`2.1.2`
-------

- **Fix:** error on adding new webhook

`2.1.1`
-------

- **Fix:** resolving name conflicts with the demo project

`2.1.0`
-------

- **Improvement:** add tokens for incoming webhooks
- **Improvement:** add helpers for one2one synchronization
- **Improvement:** show icon in app switcher in Odoo EE
- **Fix:** error on opening "Project for Unittests"
- **Fix:** Export XML: add missed fields webhook_type

`2.0.1`
-------

- **Improvement:** add the ability to get type of the given object

`2.0.0`
-------

- **Improvement:** for security sake imports are available via module code only

`1.0.0`
-------

- **Init version**
