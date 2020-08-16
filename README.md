# Hackathon Entry for [GitHub Actions Hackathon on DEV](https://dev.to/devteam/announcing-the-github-actions-hackathon-on-dev-3ljn)
**Submission Category:** 
Maintainer Must-Have

## Description of the workflow
Language Check action automatically filters issues and pull requests that contains objectionable language (profane words) and instantly reports the action URL on your chosen Slack channel. 

**This workflow is a must-have for all the developers out there who contribute to open source projects and *may* get trashed for their hard work 
🤦🏻‍♀️**

![Alt Text](https://tenor.com/view/paul-rudd-sigh-gif-5394064.gif)

**Maintaining sanity in the open source community is essential AF. 😉**

This workflow is triggered each time there is an issue is opened, or there is a new comment on an existing issue, or there is a pull request.

This workflow makes use of two already existing GitHub actions:
1. [Mind your language action](https://github.com/tailaiw/mind-your-language-action): I forked it and tweaked the `entrypoint.sh` to use conditional jobs and workflows offered by GitHub Actions API. 
2. [Slack Notify - GitHub Action](https://github.com/marketplace/actions/slack-notify): This action is highly customizable, you can send in parameters in the form of environment variables.

⚠️ To test this flow by yourself, you need to have a #blockchain channel in your workspace. Or, you can edit the `yml` file and change `SLACK_CHANNEL` there.
⚠️ You also need to generate `SLACK_WEBHOOK` token for your own Slack workspace and save it in GitHub secrets. To set it up, see [this](https://github.com/marketplace/actions/slack-notify). The slack channel I am using: degen-gh-actions.slack.com. So, the token for this workspace would be different than yours.

---

#### Feel free to reach out in case of any issue.

Cheers.✌️
