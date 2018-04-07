# How to Sync Todos from Trello to WIP

![Trello](https://notes.ciscospark.com/images/trello-logo.png)![Zapier + WIP Badge](https://emojipedia-us.s3.amazonaws.com/thumbs/120/apple/129/high-voltage-sign_26a1.png)![WIP](https://emojipedia-us.s3.amazonaws.com/thumbs/120/apple/129/construction-sign_1f6a7.png)

<br>

### What is this?
A guide on how to **automatically sync your todos** from a list in [Trello](https://trello.com/) to a product in [WIP](https://wip.chat/).

<br>

### Why?
Many WIP makers use Trello to manage our todos. This means for each task we want to work on in the near future, **we need to record that todo twice**:
1. Create a new card in your todo list in Trello.
2. Send a chat message to [@wipbot](https://t.me/wipbot) using [Telegram](https://telegram.org/) (with the same info as the Trello card) to create the todo for your product in WIP.

**Setting up this automation will remove the need for Step 2 completely.** 🙌

<br>

### How does it work?
You set create a [Zapier](https://zapier.com/) "Zap" and a [WIP Badge](https://wipbadge.com/) "Connection".
- The Zap will take each new Trello card and create a GitHub issue from it.
- The Connection will take the GitHub issue and create a WIP todo for your Product.

<br>

### Seems like a lot of moving parts...
It is. 🤷

But you set it up **once** and then it just works.

Also, [@joelbaudin](https://wip.chat/@joelbaudin) is working on a Trello integration for WIP Badge to make this easier, but until then this automation works just fine.

<br>

### How long will it take to set up, and is it free?
* **5 minutes**.
* **Yes**.

<br>

### Lets do it. 🛠️

<br>

#### Step 1: Create a GitHub repo.
> Already have a WIP Badge connection set up? **Skip to Step 3**!

✅ [Sign up here](https://github.com/join?source=header-home) for a free GitHub account if you don't already have one.

✅ [Create a new repo](https://help.github.com/articles/create-a-repo/) (This will store your todos in between Trello and WIP).
 > This repo can be private if you have a paid GitHub account, but a public repo is fine if you have a free account.
 
 1. Name the repo anything you like. For example, "**MyProductTodos**"

<br>

#### Step 2: Set up a WIP Badge connection.

✅ [Sign up here](https://wipbadge.com/signup) for a free WIP Badge account if you don't already have one.

✅ Enter and save your [WIP API Key](https://wip.chat/api) in your WIP Badge settings.

✅ Follow the WIP Badge guide to [add a connection](https://wipbadge.com/guides) from your GitHub repo to your WIP product.
> The Connection will watch for any new issues in your repo and create a new todo in WIP automatically.

<br>

#### Step 3: Create a Zap from Trello to GitHub

✅ [Sign up here](https://zapier.com/sign-up/) for a free Zapier account if you don't already have one.

✅ Follow the steps to [create this Zap](https://zapier.com/app/editor/template/563) in your Zapier account.
> The Zap will watch for any new cards you add to a specific Trello list and automatically create a new issue for each one in your GitHub repo.

1. Be sure to select `New Card` as the **Trello Trigger** and connect your Trello account.
2. After choosing your Trello Board, click `Show Advanced Options` to choose a specific list (your todo list).
3. Click `Continue` to test your Trello connection.
4. Select `Create Issue` as the **GitHub Action** and connect your GitHub account.
5. Choose your repo (**MyProjectTodos**)
6. *Set the **Title** of the Issue as the **Name** of the Trello card.*
7. Click `Send Test to GitHub` to test your GitHub connection.
8. Click `Finish` and make sure your new Zap is turned **ON**!

<br>

#### Done! 🎉

<br>

### Is that it?
Yep. Get back to work!

Continue making as you normally do, adding new todos to your Trello list.

Within 15 minutes, they **automatically appear in your product's todo list in WIP**.

<br>

### Why 15 minutes?
That's how often Zaps will check for a trigger (i.e. new Trello card). Which means usually your todos will appear in *less* than that time.

If you want to be able to mark todos as complete just a few minutes after creating them, I recommend using the usual `/done` command with @wipbot in Telegram instead.

<br>

---

<br>

#### Happy making!
#### If this automation saves you time and effort, feel free to show your support [with a cup of coffee](https://www.buymeacoffee.com/levidxyz).
#### Question / Comment? 👉 [Telegram](https://t.me/levidxyz) / [Twitter](https://twitter.com/levidxyz)
#### Levi D 🤙
