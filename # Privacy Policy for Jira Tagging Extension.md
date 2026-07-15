# Privacy Policy for Jira Tagging VN

**Last Updated: July 2026**

## 1. Overview

Jira Tagging VN is a browser extension designed to support internal Jira-based tagging workflows by providing checklist-driven sub-task creation, reusable comment templates, Jira page productivity helpers, and in-browser previews of supported Jira attachments.

The extension does not sell user data, use advertising, or transmit user data to external analytics or telemetry services.

## 2. Data Collection and Usage

Jira Tagging VN does not collect, sell, or transmit personally identifiable information (PII) to external servers or third-party services.

The extension may read Jira page content that is necessary to provide its features, including:

- Jira issue metadata and ticket context
- issue descriptions and page fields
- comment editor content
- attachment URLs and supported attachment contents
- locally created comment templates and related settings

This information is processed only to provide the extension's intended functionality.

## 3. Local Storage

User-created comment templates and related template settings are stored locally on the user's device using `chrome.storage.local`.

Temporary checklist panel state may also be stored in browser session storage.

This locally stored data remains within the user's browser unless the user manually copies, exports, or shares it outside the extension.

## 4. Jira Page Access

The extension runs only on Jira issue pages matching:

`https://jira.secext.samsung.net/browse/*`

Access is required to:

- detect the current Jira issue and workflow context
- provide checklist-driven sub-task creation tools
- insert reusable comment templates
- provide Jira page productivity helpers such as highlighting and copy actions
- preview supported Jira-hosted attachments directly in the browser

## 5. Attachment Preview Processing

When a user opens a supported attachment preview, the extension fetches the attachment directly from the Jira environment that the user is already authorized to access.

Supported attachment formats may include:

- `.msg`
- `.eml`
- `.xlsx`
- `.xlsm`

Attachment contents are processed locally in the browser for preview purposes.

The extension does not send attachment contents to third-party services, external analytics platforms, or external processing servers.

## 6. Clipboard Access

Some productivity features allow users to copy Jira-related values to the clipboard.

Clipboard actions occur only in response to explicit user interaction, such as clicking a copy button.

The extension does not continuously monitor or collect clipboard contents.

## 7. Third-Party Services and External Data Transmission

The extension does not use:

- advertising services
- analytics trackers
- telemetry services
- behavioral tracking
- external error-reporting services
- third-party data collection services

The only network requests made by the extension are those required to access Jira-hosted content, such as supported Jira attachments, within the user's authenticated Jira session.

## 8. Data Sharing and Sale

Jira Tagging VN does not sell, rent, or share user data with advertisers or third-party data brokers.

## 9. Data Retention

User-created templates and related settings remain stored locally in the browser until they are manually deleted, the extension's storage is cleared, or the extension is uninstalled.

Temporary session data is cleared according to normal browser session behavior.

## 10. Contact

Developed by **Nga Nguyen (Callie)** for internal team productivity.