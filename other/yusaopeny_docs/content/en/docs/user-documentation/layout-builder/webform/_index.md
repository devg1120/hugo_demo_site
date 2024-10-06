---
title: Webform
description: Embed an existing webform on a page.
---

{{< tabpane text=true >}}
  {{< tab header="Video" lang="vid" >}}
    {{< youtube dsHpcLDjLEo >}}
  {{< /tab >}}
  {{% tab header="Diagram" lang="pic" %}}
![Screenshot of the Webform component with block labels](lb-webform.png)
  {{% /tab %}}
{{< /tabpane >}}

-----

**Designs:**
- [Design System](../../../../../../assets/img/designs/lb-ui-kit/Forms.jpg)
- Pre-release: [Mobile](<../../../../../../assets/img/designs/lb/Webforms Mobile.png>) | [Desktop](<../../../../../../assets/img/designs/lb/Webforms Desktop.png>)

{{< readfile "../lb-add-block.partial" >}}

Fill in the content fields:

- **Title** (required): Never displayed, even if "Display Title" is checked. For administrative use only.
- **Form title**: Displayed as a heading above the item.
- **Form subtitle**: Displayed below the heading.
- **Webform** (required): Choose the Webform to embed on the page from the list of existing forms.
  - Expand **Webform settings** to access additional webform configuration, to open, close, or schedule the form.

{{< readfile "../lb-save-block.partial" >}}