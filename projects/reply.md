# REPLY · Merchant inventory & product replies

**An Arabic-first workspace that turns a product code into a clear answer.**

[Public source & documentation →](https://github.com/mohamedkbay/REPLY) · [Back to selected work](../README.md)

REPLY helps merchants organize products, prices and availability, then answer customer inquiries using product codes and saved inventory. The interface supports Arabic and English; current replies use saved rules and catalog data rather than AI-generated prices.

**Availability:** Open source · locally verified pilot; live setup still required.

## My contribution

Merchant inventory, product replies, bilingual interface and Node pilot development on an attributed open-source foundation.

## The merchant workflow

1. The merchant saves a product code, name, price, currency, availability and optional photo.
2. A customer asks about a price or sends a photo; the configured response asks for the product code.
3. A known code returns the saved product details. Unavailable products and unknown codes receive the corresponding response.
4. The merchant maintains keyword automations and editable business answers, and inspects previews and reply activity.

Incoming photos prompt code guidance; the current implementation does not identify products visually or call a language model.

## Reply in motion

[![Reply theme wave and layered menu from the actual local demo](../assets/reply/motion-preview.gif)](https://github.com/mohamedkbay/REPLY/blob/main/docs/media/Reply-Showcase.mp4)

**[Watch the full 32-second film](https://github.com/mohamedkbay/REPLY/blob/main/docs/media/Reply-Showcase.mp4)** — theme waves, layered navigation, Arabic/English switching, a product-photo reply and the responsive phone layout. The film is 1080p/30 fps; the 12-second GIF previews the theme and menu. Both use synthetic inventory and contain no live message delivery. The film is intentionally silent.

## Interface previews

![Reply inventory with explicitly labelled fictional demonstration products](../assets/reply/inventory-dark.jpg)

An existing local development capture with synthetic products and illustrative prices. This inventory capture predates the latest compact header-symbol refinement; it is not a live merchant account or a sales result.

<p align="center">
<img src="../assets/reply/login-light-mobile.jpg" width="300" alt="Reply mobile sign-in in light mode with an empty email field" />
<img src="../assets/reply/login-dark-mobile.jpg" width="300" alt="Reply mobile sign-in in dark mode with an empty email field" />
</p>

The matching sign-in captures show the English interface. Arabic RTL is the default, with English LTR, locally served Cairo, responsive layouts, light/dark modes and reduced-motion support. Email delivery is visibly disabled in these unconfigured local previews.

## Product scope

Reply extends an existing open-source automation foundation with a merchant-focused inventory workflow, product media, connected-channel adapters, bilingual interface and identity, and a separate Node customer-service pilot.

- Product codes, prices, currencies, availability, optional photos, search and list/gallery views.
- Product answers, editable business topics, keyword rules, preview and activity surfaces.
- Adapters for Instagram, Messenger, WhatsApp and Telegram; a separate, bounded TikTok workflow handles public comments on selected owned videos.
- Email-code authentication, isolated customer workspaces and limited-trial controls in the Node pilot.
- Automated tests for matching, authentication, workspace isolation, callback verification, duplicate handling and image/text fallback.

The underlying foundation is [Paul Millerd’s manychat-lite-cloudflare](https://github.com/paulmil11/manychat-lite-cloudflare), credited in the [MIT license](https://github.com/mohamedkbay/REPLY/blob/main/LICENSE) and [attribution records](https://github.com/mohamedkbay/REPLY/blob/main/NOTICE.md). This overview describes the custom extension work; it does not claim sole authorship of that foundation.

## Technology

TypeScript · Node.js · SQLite · server-rendered HTML/CSS and browser JavaScript. A separate Cloudflare Workers/D1 prototype shares the domain logic. Deployment preparation includes Docker and Caddy.

## Status and verification

**Status: open-source, locally verified pilot.** This is a product overview, not an announcement of a publicly launched service.

On 19 October 2026, a fresh local review of the uploaded snapshot passed **158 automated tests**, TypeScript checking, the Worker dry-run bundle, the Node bundle and the workerd/D1 runtime checks. Provider traffic in these tests is mocked; passing them does not establish live platform permissions or message delivery.

The latest reviewed upload, `8003132` (19 October 2026), adds the film, GIF and production notes without changing application runtime code. Media dimensions/durations, source checksums and renderer syntax were checked; the application checks above apply to the unchanged runtime.

Live enrollment still requires configured email delivery, approved platform access, public HTTPS callbacks and operational validation. The Node pilot does not yet schedule the separate daily Instagram-token renewal path. Online checkout and customer-facing paid activation are not implemented. TikTok support is public text comments on selected owned videos, not general inbox automation.

## Availability

The application source and setup guides are now [public on GitHub](https://github.com/mohamedkbay/REPLY) under the MIT license. This overview presents the product and selected development screenshots; real credentials and operational customer data are not part of the showcase. See [image sources and attribution](../assets/README.md).
