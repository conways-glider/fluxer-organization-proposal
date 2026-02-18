
# Fluxer Organization Proposal

In order to best support the development and future of Fluxer, we need a way to safely and consciously cultivate growth, proposals, and contributions. Looking at prior established organizations, we can identify some key patterns:

- Centralizing RFCs and Proposals with a common format while also supporting a centralized product vision.
- Centralizing issues and bugs to support a common report path.
- Creating a consistent and actionable organization structure that is capable of supporting multiple independent actors.
- Enabling community contributions, both by open-source and community support.
- Designing Processes, Platforms, and Organization around flexible growth.

Most notably, enabling the central vision of Hampus while also supporting community input should be our principle goal.

To enable this, I propose the following:

- Establishing Community Code of Conduct for Contributors
- Creating Common Patterns for Discussions
- Establishing Working Groups
- Compensation for Developers

## Establishing Community Code of Conduct for Contributors
This is most notably exemplified by the growth of the Rust and Zig Languages. By establishing a strong Code of Conduct, they were able to cultivate an inclusive community by declaring intention at the forefront of our community, ensuring people feel safe to contribute and that exclusive behavior can be prevented.

To be clear, this Code of Conduct should be for the Fluxer Organization for contributions. Some of these guidelines may not be appropriate for the Fluxer Platform/Application, as servers should develop their own code of conduct.

Common Codes of Conduct can be found to have the following principles:

- Inclusiveness around characteristics (Gender, Race, Sexuality, Disability, Religion, etc.).
  - This is not an exclusive list and should be expanded upon prior to publishing any Code of Conduct.
- Ensuring topics remain on topic and respectful.
- Assuming kindness in interactions.
- Respecting differences of opinion.
  - This is important as Fluxer grows, many decisions won't please everyone. We should acknowledge that every decision has tradeoffs and that many decisions don't have a right answer, but still need a decision made.
- Ensuring all criticism has a purpose. Vague Criticism is unproductive and can lead to harming others within discussions.
- Taking a stance on the "Paradox of Intolerance". This could also be phrased as intentional, extreme, or repetitive violations of the Code of Conduct can lead to being "timed-out", suspended from discussions, or blocked from contribution.
  -  This should also be taken as notice that if you harass or demean members and contributors or troll discussions, you may be excluded for the safety of the community.

These guidelines are derived from successful organizations and should be a guiding principle while writing our Code of Conduct.

Additionally, we should also establish a way to report violations of the Code of Conduct such that users can ensure a safe community. Common methods for this are establishing an email address or other outside standards. This ensures that even in the case of system downtime, these reports are not lost.

## Creating Common Patterns for Discussions

Fluxer is currently hosted on GitHub, which has a wealth of support for Issues, Discussions, and Contributions. For proposals of features or changes, we should consider creating an Request for Comment (RFC) based system, where users can comment on proposals prior to committing to a design or feature and users can openly create proposals.

To best support the openness of a full RFC Process, we should create a new git repository to host proposals. 

This repository would contains:

- All Submitted RFCs, whether accepted or rejected.
- A Standard RFC Format that users can base suggestions on.
  - Pull Requests would be the hub of discussion around RFCs. This allows for complete openness of direction and maintaining an open history of discussion.
- Guidelines for Reopening or Reworking Closed RFCs.

## Establishing Working Groups

As the platform grows, a single developer or a disorganized group of organizers quickly becomes a unsustainable solution. The most common pattern to solve this is to create Working Groups. These groups can own a problem domain on their own and have a minor degree of autonomy while establishing goals, timelines, and direction.

This also allows for Hampus and any core architects to still have necessary oversight and direction while also delegating work to allow for a sustainable workload.

A possible structure of this could be:

- Core Platform
- Web & Desktop Interface
- Mobile Interfaces
- Infrastructure
- Self-Hosted Support

Each working group should have a Lead and a Co-Lead, initially through nomination, but later on, groups could elect their own leaders. These Leads would be able to own a problem domain and allow Hampus to delegate as the problems grow in scale.

## Compensation for Developers

To best support the longevity of contributors, we should consider compensation for major contributions. This however presents a few problems:

- How do we sustainably support developers while also operating in a way that ensures continued operations and viability of the parent organization?
- How do we transition this in the long-term when Fluxer grows?
- How do we prevent abuse of a bug-bounty or contributor compensation program?

To best reward contributors for their time, we should consider a standard system:

1. Security Risk Bug Bounties
2. Pre-Allocated Contribution Compensation
3. Organization Promotion and Hiring

