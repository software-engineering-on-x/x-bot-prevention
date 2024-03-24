# 𝕏 Bot Prevention <!-- omit in toc -->

![build](https://img.shields.io/github/actions/workflow/status/software-engineering-on-x/x-bot-prevention/ci.yml?branch=master)
[![xbotprevention: rustc 1.77+](https://img.shields.io/badge/xbotprevention-rustc_1.77+-lightgray.svg)](https://blog.rust-lang.org/2024/03/21/Rust-1.77.0.html)

An X bot that analyzes spam bots and blocks them from following, responding etc to an account.

## About

The idea of this tool is to prevent spam bots on X to follow, respond, like or interact with an account to not mark the targeted
account a lower score.

### Key factors 

Some of the key factors with its probability (0-1) that the bot will evaluate if the account is a spam bot account:

- 0 followers
- Only followed by unverified
- No posts or only re-posts
- No media
- No profile picture
- Gif spam
- No description
- Duplicated description based on other account that exists in current dataset
- No banner
- Sending only duplicated posts to multiple accounts

These factors will be saved in a configuration file that will be loaded on runtime. Check the configuration file here: [Settings.toml](backend/Settings.toml)

## Technologies

More will come later...

- [sqlx (sqlite)](https://github.com/launchbadge/sqlx)
- [twitter-v2-rs](https://github.com/jpopesculian/twitter-v2-rs)

## Getting Help

Are you having trouble with 𝕏 Bot Prevention? We want to help!

- Ask questions about it in the Software Engineering community.

- Report bugs at https://github.com/software-engineering-on-x/x-bot-prevention/issues.

## Reporting Issues

𝕏 Bot Prevention uses GitHub’s integrated issue tracking system to record bugs and feature requests. If you want to raise an issue, please follow the recommendations below:

- Before you log a bug, please search the issue tracker to see if someone has already reported the problem.

- If the issue doesn’t already exist, create a new issue.

- Please provide as much information as possible with the issue report. We like to know the 𝕏 Bot Prevention version, operating system, and Rust version version you’re using.

- If you need to paste code or include a stack trace, use Markdown. ``` escapes before and after your text.

- If possible, try to create a test case or project that replicates the problem and attach it to the issue.

## Code of Conduct

Anyone who interacts with 𝕏 Bot Prevention in any space, including but not limited to this GitHub repository, must follow our code of conduct.

## Contributors

The following contributors have either helped to start this project, have contributed
code, are actively maintaining it (including documentation), or in other ways
being awesome contributors to this project. **We'd like to take a moment to recognize them.**

[<img src="https://github.com/mjovanc.png?size=72" alt="mjovanc" width="72">](https://github.com/mjovanc)

## License

The GPLv3 License.
