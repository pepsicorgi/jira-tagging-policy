# Privacy Policy for Jira Tagging VN

**Last Updated: September 2026**

## 1. Overview

Jira Tagging VN is a browser extension designed to support internal web tagging and analytics QA workflows. It provides Jira-based workflow helpers, reusable comment templates, attachment previews, implementation-guide handling, and in-browser validation of tagging implemented on supported Samsung websites.

The extension does not sell user data, use advertising, or transmit user data to the developer, external analytics services, telemetry services, or data brokers.

## 2. Data Processed by the Extension

Jira Tagging VN processes only the information needed to provide its user-facing features. Depending on the feature being used, this may include:

- Jira issue metadata, ticket context, descriptions, page fields, and comment-editor content
- Jira attachment URLs and the contents of supported attachments selected by the user
- user-created comment templates and related settings
- implementation-guide files and parsed guide content imported by the user
- Samsung page URLs and selected DOM content such as tagging attributes, text, links, element state, and interaction context
- Adobe Analytics tagging data observed during a user-initiated validation run, including Rule names, events, eVars, props, request URLs, and request payload data required for validation

The extension may incidentally process personal or sensitive information if that information is present in Jira content, email attachments, implementation guides, website content, or analytics payloads. The extension does not use such information for profiling, advertising, marketing, or unrelated purposes.

## 3. Jira Page Access

The extension runs on supported Jira issue pages, including:

`https://jira.secext.samsung.net/browse/*`

Jira page access is used to:

- detect the current Jira issue and workflow context
- provide checklist-driven sub-task and tagging-support helpers
- insert reusable comment templates
- provide productivity features such as highlighting and copy actions
- preview supported Jira-hosted attachments directly in the browser

Jira content is processed only to provide these features.

## 4. Samsung Website QA and Tagging Validation

The QA module runs on supported Samsung websites when the user uses the QA interface.

For a user-initiated validation, the extension may inspect the current page and selected interaction context, including:

- page URL
- selected or interacted DOM elements
- tagging attributes such as `an-tr`, `an-ca`, `an-ac`, `an-la`, and related supported attributes
- element text, links, accessibility labels, and state needed to evaluate implementation-guide requirements

This information is used only to compare the implemented tagging against the selected or imported implementation guide.

## 5. Adobe Analytics Request Inspection

During an active QA validation run, the extension may observe Adobe Analytics network traffic sent by the Samsung page to supported Adobe collection endpoints, including `smetrics.samsung.com`.

The extension may inspect request metadata and payload fields needed for validation, such as:

- Adobe Rule names
- analytics events
- eVars
- props
- request URLs and request identifiers
- related XDM/request payload content needed to determine whether expected tagging was sent

The extension uses this information only to provide the user-facing tagging validation result. It does not block, modify, or redirect Adobe Analytics requests.

Validation payload evidence is processed locally in the browser and is not transmitted by the extension to the developer or to an external analytics or telemetry service.

## 6. Implementation Guides and Sample Guides

The extension may allow users to import supported implementation-guide files, including presentation files used for tagging QA.

Imported guide content may be parsed locally to extract requirements, examples, notes, and related validation information. Parsed guide data may be stored locally in the browser so that the user can reuse it during the QA workflow.

The extension also includes built-in sample guide presets packaged with the extension. These presets are local configuration data and do not require an external service.

## 7. Local and Session Storage

The extension uses browser-local storage only for functionality required by the extension.

Examples include:

- user-created Jira comment templates and related settings stored with `chrome.storage.local`
- temporary QA and validation session state stored with `chrome.storage.session`
- imported or parsed implementation-guide data stored locally in browser storage such as IndexedDB

Validation request payload evidence used during an active run is intended to remain temporary and is not used for developer telemetry.

Locally stored data remains within the user's browser unless the user manually copies, exports, shares, or otherwise transfers it outside the extension.

Users can remove locally stored extension data by using available extension controls where provided, clearing extension/browser storage, or uninstalling the extension.

## 8. Attachment Preview Processing

When a user opens a supported Jira attachment preview, the extension fetches the selected attachment directly from the Jira environment that the user is already authorized to access.

Supported formats may include:

- `.msg`
- `.eml`
- `.xlsx`
- `.xlsm`
- other supported document formats used by the extension

Attachment contents are processed locally in the browser for preview purposes and are not uploaded by the extension to an external processing service.

Email attachments may contain remote images or other externally hosted resources. If such a resource is rendered by the browser while the user views the preview, the browser may contact the external host referenced by the email. This behavior originates from the content of the email and is not used by Jira Tagging VN for analytics, advertising, or telemetry.

## 9. Clipboard Access

Some productivity and QA features allow users to copy values or validation results to the clipboard.

Clipboard actions occur only in response to explicit user interaction, such as clicking a Copy button.

The extension does not continuously monitor or collect clipboard contents.

## 10. Network Access and External Services

Jira Tagging VN does not use:

- advertising services
- developer-operated analytics trackers
- telemetry services
- behavioral advertising or profiling services
- external error-reporting services
- third-party data brokers

Network access is limited to functionality required for the extension's user-facing purpose, including:

- accessing Jira-hosted pages and attachments within the user's authenticated Jira session
- operating on supported Samsung pages
- observing Samsung-page Adobe Analytics requests during user-initiated QA validation
- browser loading of remote resources referenced by user-opened content, such as remote images in email previews, where applicable

The extension does not send captured Jira, Samsung-page, guide, attachment, or Adobe Analytics validation data to the developer's own server.

## 11. Data Sharing and Sale

Jira Tagging VN does not sell, rent, or share user data with advertisers or third-party data brokers.

Data processed by the extension is used only to provide or improve the extension's disclosed internal tagging and QA functionality.

## 12. Data Retention

Retention depends on the type of data:

- user-created templates and related local settings remain in browser storage until deleted, browser extension storage is cleared, or the extension is uninstalled
- imported or parsed guide data stored locally remains until removed by the user, cleared from browser storage, expired according to the extension's local cache behavior, or the extension is uninstalled
- temporary QA session state is retained only for the browser session or according to the extension's session/cache behavior
- validation request evidence is intended to be temporary and used only for the active validation workflow

The extension does not maintain a developer-operated server-side database of this information.

## 13. Limited Use

Data accessed by Jira Tagging VN is used only to provide and improve its disclosed user-facing tagging-support and QA functionality.

The extension does not use accessed data for advertising, creditworthiness, lending, unrelated profiling, sale, or other purposes unrelated to the extension's stated functionality.

## 14. Security

The extension is built as a Manifest V3 Chrome extension and packages its executable extension code locally. It does not intentionally load or execute remotely hosted JavaScript.

Access to Jira and Samsung resources is limited to the permissions and host access required by the extension's functionality.

## 15. Changes to This Policy

This Privacy Policy may be updated when the extension's functionality or data-handling practices change. The "Last Updated" date above reflects the latest revision.

## 16. Contact

Developed by **Nga Nguyen (Callie)** for internal team productivity and tagging QA workflows.
