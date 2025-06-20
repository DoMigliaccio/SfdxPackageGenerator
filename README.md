# 🛠️ Salesforce Package XML Generator Plugin

Build your XML package for your Salesforce deploys!  
With this plugin, you can retrieve metadata resources and quickly generate the contents of the 📦`package.xml`📦 file for your Salesforce project deployments.

---

## 🚀 Features

- **Automatic Org Selection**: Start by choosing the org you want to retrieve resources from. The list is automatically built from the connections in your CLI.
- **Predefined Metadata Types**: A default list of metadata types is provided for retrieval.
- **Customizable**: Need more types? Easily edit the list from the plugin settings.
- **Interactive Selection**: Once the retrieval is done, select the resources you need.
- **Live Preview**: Preview the package progress in the side panel.
- **Easy Copy**: Copy the content to your clipboard and paste it into your `package.xml` file.

✨ Just like that, your file for migrating resources between orgs is ready.

---

## ⚙️ Setup & Configuration

After installing the plugin, make sure the setup is complete:

1. Open **Settings > Tools > Salesforce Package Generator Settings**.
2. Check the installation path for `SF.cmd` (or `SFDX.cmd`).
3. If the path is incorrect or empty, update it with the correct installation path on your PC.

---

## 📦 Example

```xml
<?xml version="1.0" encoding="UTF-8"?>
<Package xmlns="http://soap.sforce.com/2006/04/metadata">
    <types>
        <members>*</members>
        <name>ApexClass</name>
    </types>
    <version>59.0</version>
</Package>
