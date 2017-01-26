## SplitViewController, TabViewController, and MapKit- Create an app to view websites and their locations

You can use the [editor on GitHub](https://github.com/zsheill7/SwiftTutorial/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

What is Firebase?

Firebase is a realtime database that you can communicate with to handle authentication, push notifications, advertisements and more.  In this tutorial, you will learn how to use Firebase to sign up users with different traits and view them all in a table.  

To create an account, visit the Getting Started page and log in with your Google account.  This tutorial will only require a free plan.

![Screenshot 1](/images/FireShot 1.png)

To begin creating your first project click CREATE NEW PROJECT.  

![Screenshot 3](/images/FireShot 3.png)

Enter "FriendChat" (or another name if you prefer) in the "Project Name" field and enter your country.

![Screenshot 4](/images/FireShot 4.png)

Enter com.friendchat.app in the "iOS Bundle ID" field. 

![Screenshot 6](/images/FireShot 6.png)

A Google-Info.plist file will be downloaded when you click "ADD APP."  Be sure to save this, as you will need it later. 

![Screenshot 8](/images/FireShot 8.png)
![Screenshot 9](/images/FireShot 9.png)


With your Firebase app set up, go to Xcode and open LoginViewController.swift. Where the variables are defined at the top, add the following:
let ref = FIRDatabase.database().reference(withPath: "users")

This reference lets you connect to your Firebase database to store and retrieve users.  The "withPath" part refers to a location in your Firebase database.

The data is stored as JSON in a key-value structure.  Every key may correspond to several values.  For example, every user (the key being their unique ids) can have a different birthday and gender (values).  The data can be a number, string, boolean or object.


Below is a simple firebase database that includes two users, user1 and user2, with different properties of both. 

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/zsheill7/SwiftTutorial/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
