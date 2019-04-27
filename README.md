# Translations

Translations of Dir

# Translation Guide

## 0x01 Folders

Folders in root are different locales. Format: `value-<language code>`, for instance:

The language code of Chinese (Taiwan) is `zh-rTW`, so the folder name should be: `values-zh-rTW`. For default locale, which is English in this situation, has the name of `values`. 

## 0x02 Inside the folder

Inside the folder are the `strings.xml` file. You should NOT place any other files in these folders. 

## 0x03 The XML

The XML is Android Resources XML file. For more information, take a look at online documents. There is a brief introduction of them. 

```xml
<!-- Keep these two lines -->
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <!-- Add a String resource which has the name of "my_key" and its value (which will be displayed in most of the cases) is "My Value". -->
    <string name="my_key">My Value</string>
    <!-- Add another String resource -->
    <string name="my_name">YuutaW</string
</resources>
```

In this situation, you should not add any other keys and need to **override** the existing keys from the default locale file and translate them to your selected language. All strings which are NOT overridden by exactly the same key will be falled back to the default value.

In the example below, some texts are wrapped in `<!-- some text -->`. These texts are comments which is used to help you understand and will NOT be included in final builds, you can ignore them.

**IMPORTANT**: You should ALWAYS translate from the default values which is English in this project. The developer will ALWAYS update the default values XML at first.

## 0x04 Start translating

You now know the necessary essential knowledge about translating. Pick one of your prefered language and start translating now! You'll need to create a PR (Pull Request) to submit them. 

## 0x05 Fork & Pull Request

You'll need to `Fork` (not fu*k :D) this repo to your own GitHub account. You can just click the `Fork` button on the right top conner of the repo.

After forking, you can start translating. After you had done, `commit` your changes by using Git. If you are not familiar with `git` command, just add your translated file online by clicking `Create new file` and put your translated XML inside.

Now, your translation is available so you are ready to create a Pull Request. You just need to click on the `Pull request` button and confirm creating a new PR. Our admins will review your translation later.

# Licenses

You have no permission republishing any source codes in this Repo because it's a part of private software.
