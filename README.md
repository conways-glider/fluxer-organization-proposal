# Fluxer Organization Proposal

In order to best support the development and future of Fluxer, we need a way to safely and consciously cultivate growth, proposals, and contributions. Looking at prior established organizations, we can identify some key patterns:

- Centralizing RFCs and Proposals with a common format while also supporting a centralized product vision.
- Centralizing issues and bugs to support a common report path.
- Creating a consistent and actionable organization structure that is capable of supporting multiple independent actors.
- Enabling community contributions, both by open-source and community support.
- Designing Processes, Platforms, and Organization around flexible growth.

Most notably, enabling the central vision of Hampus while also supporting community input should be our principal goal.

To enable this, I propose the following:

- Establishing Community Code of Conduct for Contributors
- Defining Governance and Decision-Making
- Creating Common Patterns for Discussions
- Establishing Working Groups
- Contributor Onboarding
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
  - This should also be taken as notice that if you harass or demean members and contributors or troll discussions, you may be excluded for the safety of the community.
- NSFW topic discussion should be considered "Off-Limits" in official communications, repositories, issues, RFCs, or RFC Discussions.

These guidelines are derived from successful organizations and should be a guiding principle while writing our Code of Conduct.

Additionally, we should also establish a way to report violations of the Code of Conduct such that users can ensure a safe community. Common methods for this are establishing an email address or other outside standards. This ensures that even in the case of system downtime, these reports are not lost.

## Defining Governance and Decision-Making

For Fluxer to grow sustainably, we need a clear governance model that preserves Hampus's vision while empowering contributors to take ownership of their work. To achieve this, Hampus should serve as the project's Benevolent Dictator for Life (BDFL), retaining final authority over the project's direction while formally delegating specific domains to Working Group leads.

This model is well-established in open-source, most notably by Python under Guido van Rossum's leadership. It provides clarity on who makes decisions and prevents governance ambiguity from stalling progress.

### Decision Authority

Under this model, decision-making would be structured as follows:

- **Hampus (BDFL)**: Retains final authority over project direction, core architecture, and any decisions that span multiple Working Groups. Can delegate decision-making power to Working Group leads and revoke it if necessary.
- **Working Group Leads**: Have binding decision-making authority within their delegated domain. This includes implementation details, prioritization of work within the group, and domain-specific technical decisions.
- **Contributors**: Can propose changes through the RFC process and participate in discussions. All contributors have a voice, but decision-making authority flows through the structures above.

### RFC Approval

RFCs that fall within a single Working Group's domain can be approved by that group's lead. RFCs that affect multiple groups or core architecture require Hampus's approval. In cases where scope is ambiguous, Working Group leads should escalate to Hampus.

### Conflict Resolution

Disputes between contributors, or between Working Groups, should first be resolved through discussion among the involved parties. If no resolution is reached, the dispute should be escalated to Hampus for a final decision.

As the organization matures and Working Group leads gain experience, we should consider transitioning to a lead council model where Working Group leads vote on cross-cutting disputes, with Hampus serving as tiebreaker. This transition should happen organically as trust and processes solidify, rather than being forced prematurely.

## Creating Common Patterns for Discussions

Fluxer is currently hosted on GitHub, which has a wealth of support for Issues, Discussions, and Contributions. For proposals of features or changes, we should consider creating a Request for Comment (RFC) based system, where users can comment on proposals prior to committing to a design or feature and users can openly create proposals.

To best support the openness of a full RFC Process, we should create a new git repository to host proposals.

This repository would contain:

- All Submitted RFCs, whether accepted or rejected.
- A Standard RFC Format that users can base suggestions on.
  - Pull Requests would be the hub of discussion around RFCs. This allows for complete openness of direction and maintaining an open history of discussion.
- Guidelines for Reopening or Reworking Closed RFCs.

Once an RFC has been accepted, the intended architecture and spec should be written up and created as an Issue on the GitHub Repository.

### Roadmap & Prioritization

Accepted RFCs need to be prioritized against each other to form a coherent roadmap. Without this, accepted proposals can pile up with no clear order of execution, leaving contributors uncertain about where to focus their efforts.

Hampus should maintain a public roadmap that reflects the current priorities of the project. This roadmap should be informed by accepted RFCs, bug reports, and the needs of each Working Group. Working group leads should actively participate in prioritization by surfacing the needs of their domain, flagging dependencies, and proposing ordering within their area of ownership. Final prioritization decisions, especially those that span multiple groups or affect the project's overall direction, rest with Hampus.

The roadmap should be reviewed on a regular cadence and updated as priorities shift. Transparency here is important, contributors and the community should be able to see what's being worked on, what's coming next, and what has been deferred. A simple GitHub Project board or a dedicated page in the RFC repository would be sufficient for this purpose.

## Establishing Working Groups

As the platform grows, a single developer or a disorganized group of organizers quickly becomes an unsustainable solution. The most common pattern to solve this is to create Working Groups. These groups can own a problem domain on their own and have a minor degree of autonomy while establishing goals, timelines, and direction.

This also allows for Hampus and any core architects to still have necessary oversight and direction while also delegating work to allow for a sustainable workload.

A possible structure of this could be:

- Core Platform
- Web & Desktop Interface
- Mobile Interfaces
- Infrastructure
- Self-Hosted Support

Each Working Group should have a Lead and a Co-Lead, initially through nomination, but later on, groups could elect their own leaders. These Leads would be able to own a problem domain and allow Hampus to delegate as the problems grow in scale.

### Working Group Communication

Each Working Group should have dedicated communication channels for coordination hosted on a Fluxer instance. This serves both as a practical tool for real-time discussion and as a demonstration of the platform itself.

At minimum, each Working Group should maintain:

- A dedicated channel for day-to-day discussion and coordination.
- A regular sync cadence to align on priorities and surface blockers.
- A channel for community members to ask questions or follow along with the group's work.

Beyond the Working Groups, we should also provide a general development channel for broad questions and discussion, as well as a channel for newcomers to introduce themselves and ask for guidance.

Cross-group coordination should also have a dedicated space where Working Group leads can discuss issues that span multiple domains, such as shared API changes or release planning.

## Contributor Onboarding

Growing a healthy contributor community requires making newcomers feel welcome and giving them a clear path to their first contribution. Without intentional onboarding, new contributors often struggle to find where they can help, feel intimidated by unfamiliar codebases, or leave after a poor first experience.

### Good First Issues

We should maintain a curated set of issues labeled "Good First Issue" across Fluxer's repositories. These issues should be well-scoped, clearly described, and approachable without deep knowledge of the codebase. Working group leads should be responsible for identifying and labeling these within their domains.

Good first issues serve a dual purpose:

- They provide an entry point for new contributors.
- They surface smaller tasks that experienced contributors often overlook.

### Mentorship

New contributors should have access to guidance from experienced members of the community. Working group leads and co-leads should be available to answer questions and provide direction for contributors working within their domain.

As the community grows, we should consider establishing a mentorship program where experienced contributors can volunteer to guide newcomers through their first contributions. This doesn't need to be formal initially, even pointing someone to the right file or explaining a design decision can make the difference between a contributor staying or leaving.

### Contributing Guide

Each repository should include a contributing guide that covers the basics: how to set up a development environment, how to run tests, coding conventions, and how to submit a pull request. This guide should be kept up to date by the relevant Working Group and reviewed periodically to ensure accuracy.

## Compensation for Developers

To best support the longevity of contributors, we should consider compensation for major contributions. This however presents a few problems:

- How do we sustainably support developers while also operating in a way that ensures continued operations and viability of the parent organization?
- How do we transition this in the long-term when Fluxer grows?
- How do we prevent abuse of a bug-bounty or contributor compensation program?

To best reward contributors for their time, we should consider a standard system:

1. Pre-Allocated Contribution Compensation
2. Security Risk Bug Bounties
3. Organization Promotion and Hiring

### Pre-Allocated Contribution Compensation

For accepted RFCs, large feature additions, or major refactors, Hampus or the Fluxer Organization can establish pre-allocated rewards for contributions.

This should be visible ahead of time as an Issue label. To maintain community trust, changing the value of Contributions should be avoided, as work may be underway when values are changed, and decreasing value after work starts erodes community trust and disincentivizes future contributions.

At a starting point, values should remain small as to not over-extend Hampus or the Fluxer Organization, however as the Organization grows, values can be increased incrementally.

To handle maintaining this program, tools such as [Open Collective](https://opencollective.com) or [Algora](https://algora.io/) should be considered as a disbursement method and management tool.

### Security Risk Bug Bounties

Maintaining a Bug Bounty or Security Risk Bounty program can bring value long-term to projects, however, they also bring a high management burden and are often susceptible to abuse. We should consider hosting a Bug Bounty program, but at a later stage.

Considering the recent difficulty in managing these, as seen by the [curl maintainers](https://daniel.haxx.se/blog/2025/07/14/death-by-a-thousand-slops/), we should defer on creating a bug bounty until a later time when we have the resources to successfully manage the program.

### Organization Promotion and Hiring

When the Fluxer Organization is financially capable of on-boarding part-time or full-time employees, we should consider contributions as a potential source of candidates. Being transparent about this early on can help create trust in the Developer Community. We should be careful though of any messaging around this initiative and be clear that this is an eventual goal of the Organization and not something we're imminently planning.

## Frequently Asked Questions

### Will the Code of Conduct apply to servers hosted on Fluxer?

No, while maintaining a separate Code of Conduct for the Fluxer Instance hosted by Hampus and the Fluxer Organization may be important, this proposed Code of Conduct is for the Organization itself.

Additionally, self-hosted servers should develop their own Codes of Conduct as they decide what is appropriate in their environments.

### Can Hampus override or veto an accepted RFC?

Yes. As the BDFL, Hampus retains final authority over all project decisions, including the ability to override or veto an accepted RFC. This should be exercised sparingly and with clear reasoning communicated to the community. The RFC process exists to surface the best ideas and build consensus, but ultimately the project's direction must remain aligned with its core vision. If an override occurs, the reasoning should be documented on the RFC itself so the community understands the decision.

### How are Working Group leads selected?

Initially, Working Group leads and co-leads will be nominated by Hampus based on demonstrated contribution and domain expertise. As the organization matures and Working Groups become more established, groups should transition to electing their own leaders from within their membership. The specifics of an election process should be defined collaboratively once the organization reaches that stage.

### What happens if a Working Group lead becomes inactive or ineffective?

If a Working Group lead is unable to fulfill their responsibilities, whether due to inactivity, burnout, or other reasons, the co-lead should step into the role. If both the lead and co-lead are unavailable, Hampus can appoint an interim lead. We should approach these situations with empathy. Contributor burnout is common in open-source, and stepping down should be treated as a normal and respected part of participation, not a failure.
