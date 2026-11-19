# Music Assistant - Community Catalog Rules

The community catalog is a list of music sources, players and plugins that people from the community build and maintain. Each one lives in its maintainer's own public repository, under an open source licence. An administrator can enable the community catalog in the Marketplace of Music Assistant and install from it.

The [usage policy](https://github.com/music-assistant/.github/blob/main/USAGE_POLICY.md) describes what the project itself ships. For what others add to the community catalog, the lines on this page apply.

## What being listed means

A listed provider was accepted for what it does, and every release of it is checked automatically: that it loads, and that it stays within the lines below. That is all it means. The Music Assistant project does not review its code, does not test whether it works and does not support it.

A community provider runs as part of your Music Assistant server, with the same access the server has. You install it at your own risk, and its maintainer is the one to ask when something does not work.

## What is not accepted

A provider is declined when it is submitted, and blocked when it is found later, if it:

- gives access to music the user has no right to, by getting around an account, a subscription tier or regional availability, or by using a source that offers music without the rights holders' permission;
- gets around copy protection to give more than the service's own app gives the user's account;
- downloads or exports music to keep it (a temporary cache that is only used for playback is fine);
- harms the user, by sending their data anywhere but the service it connects to, by loading code from somewhere else while it runs, or by doing things its description does not mention;
- offers AI assistants tools whose description or results do more than describe the tool and report what it did, such as instructing the assistant about other tools, the user or the conversation;
- mainly exists to load other providers, or third-party lists of sources, from outside the community catalog.

## What is allowed

As long as it stays within the lines above, a provider may, at the user's own risk:

- be of use to only a few people;
- work like the service's own app does for the user's own account, also by reverse engineering it: an unofficial API, or decoding protected audio to play it;
- read a service's public web pages;
- play free public content, in the quality the service offers without a subscription;
- have code that would not pass review for Music Assistant itself.

An unofficial API, decoding a service's audio or reading its web pages can be against the service's terms and can put your account at risk. Being listed does not change that: whether you use such a provider is your own decision.

## Getting a provider listed

Start from the [provider template](https://github.com/music-assistant/community-provider-template): it holds a working example, its tests and the checks every release gets. When your provider works and you have published a release, submit it with the form [Submit a provider](https://github.com/music-assistant/community-catalog/issues/new?template=submit-provider.yml); the README of the [registry](https://github.com/music-assistant/community-catalog) says what it needs. When every check passes, a registry maintainer decides once, about what the provider does, against the lines on this page. After that you release whenever you want: every release is checked automatically and reaches users without waiting for anyone.

## Reporting a provider

If a listed provider crosses one of the lines above, report it with the form [Report or change a provider](https://github.com/music-assistant/community-catalog/issues/new?template=report-provider.yml). Say which provider it is, what it does and how you noticed.

If a provider puts its users at risk, do not post the details in public. Report it through "Report a vulnerability" on the Security tab of the registry instead. The Music Assistant team uses such a report only to hold back a release or block the provider.

## What happens to a blocked provider

- It is marked as blocked in the list, with the reason.
- Servers pick that up at their next daily check and stop loading it. The administrator sees why. Its settings and library items are kept.
- Its maintainer can ask for it to be listed again once the cause is fixed.
