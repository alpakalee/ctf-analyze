---
description: Inject JavaScript code on victims to perform actions on their behalf
---

# Cross-Site Scripting (XSS)

## Related Pages

* [JavaScript](../../../languages/javascript/)

## Description

Cross-Site Scripting (XSS) is a vulnerability that allows attackers to inject and execute malicious JavaScript code in a victim's browser.

### Types of XSS

* **Reflected XSS**: Payload is reflected from a URL parameter
* **Stored XSS**: Payload is stored on the server and executed later
* **DOM XSS**: Payload exploits client-side JavaScript vulnerabilities

## Basic Example

```html
<!-- Vulnerable Code -->
<p><?php echo $_GET["input"]; ?></p>

<!-- Attack -->
http://example.com/page?input=<script>alert(document.cookie)</script>
```

---

**Note**: This is a simplified version. Full content will be added gradually.
