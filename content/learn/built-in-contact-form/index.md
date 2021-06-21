---
title: "Built-in Contact Form"
subtitle: "Form to email feature powered by Formspree"
excerpt: "This theme has a form-to-email feature built in, thanks to the simple Formspree integration. All you need to activate the form is a valid recipient email address saved in the form front matter."
date: 2019-07-01
author: "Eric Anderson"
draft: false
tags:
  - hugo-site
categories:
  - Theme Features
# layout options: single, single-sidebar
layout: single
---

![Formspree Logo](formspree-logo.png)

## [Formspree](https://formspree.io) makes it easy to receive submissions from HTML forms on your static website.

---

### Functional Form

This theme has a **form-to-email** feature built in, thanks to the simple Formspree integration. First, [login](https://formspree.io/login) to your existing account or [register](https://formspree.io/register) for a new account at Formspree. Then create a new form in Formspree. Open Details -> Integration and you would see endpoint of your newly-created form. It is like https://formspree.io/f/xxxxxxxx. Note your Formspree form id (xxxxxxxx).

Now edit the form front matter (`/content/forms/contact.md`) and use your Formspree form id in the part asking for formspree_form_id.

```toml
# please replace with a valid Formspree form id
formspree_form_id: xxxxxxxx
```

Update that file and you're ready to begin receiving submissions.The next time someone
fills it out, the submission will land in your inbox.

### Multiple Layouts

The files included with the theme have a contact page ready for copy/paste, or
you can type `hugo new forms/contact.md` and you're off to the races. There are two
layouts for `forms` – `split-right`, and `split-left` – you guessed it, one puts
the form on the right and the other on the left. You just fill out the front
matter, and the rest is automatic.

```toml
# layout options: split-right or split-left
layout: split-right
```

![Contact Form Split Right Layout Screenshot](built-in-contact-form-screenshot.png)

Both layouts display the page title and description opposite the form, and you
can also choose to show your social icon links if you have those configured in
the `config.toml` file.
