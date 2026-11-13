# Music Assistant - Community Catalog Rules

> The community catalog is being built and does not accept providers at this moment.

The community catalog is a list of music sources, players and plugins that people from the community build and maintain. Each one lives in its maintainer's own public repository, under an open source licence. An administrator can switch the community catalog on in Music Assistant and install from it.

The [usage policy](https://github.com/music-assistant/.github/blob/main/USAGE_POLICY.md) describes what the project itself ships. For what others add to the community catalog, the lines on this page apply.

## What being listed means

A listed provider was accepted for what it does, and every release of it is checked automatically: that it loads, and that it stays within the lines below. That is all it means. The Music Assistant project does not review its code, does not test whether it works and does not support it.

A community provider runs as part of your Music Assistant server, with the same access the server has. You install it at your own risk, and its maintainer is the one to ask when something does not work.

## What is not accepted

A provider is declined when it is submitted, and blocked when it is found later, if it:

- gives access to music the user has no right to, by getting around an account, a subscription tier or regional availability, or by using a source that offers music without the rights holders' permission;
- circumvents copy protection;
- downloads or exports music to keep it (a temporary cache that is only used for playback is fine);
- harms the user, by sending their data anywhere but the service it connects to, by loading code from somewhere else while it runs, or by doing things its description does not mention;
- mainly exists to load other providers, or third-party lists of sources, from outside the community catalog.

## What is allowed

As long as it stays within the lines above, a provider may, at the user's own risk:

- be of use to only a few people;
- use an unofficial API with the user's own account, for what that account may play;
- read a service's public web pages;
- play free public content, in the quality the service offers without a subscription;
- have code that would not pass review for Music Assistant itself.

An unofficial API or reading web pages can be against a service's terms and can put your account at risk. Being listed does not change that: whether you use such a provider is your own decision.

## Reporting a provider

If a listed provider crosses one of the lines above, open an issue in the [registry](https://github.com/music-assistant/community-catalog/issues). Say which provider it is, what it does and how you noticed.

If a provider puts its users at risk, do not post the details in public. Report it through "Report a vulnerability" on the Security tab of the registry instead.

## What happens to a blocked provider

- It is marked as blocked in the list, with the reason.
- Servers pick that up at their next daily check and stop loading it. The administrator sees why. Its settings and library items are kept.
- Its maintainer can ask for it to be listed again once the cause is fixed.
