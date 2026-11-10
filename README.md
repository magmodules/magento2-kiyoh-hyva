<img width="924" alt="hyva-kiyoh-magento" src="https://github.com/magmodules/magento2-kiyoh-hyva/assets/24823946/b326c8ad-e3e2-4c6b-a8c7-255de8f8a813">

# Kiyoh Hyvä Compatibility plugin

The Kiyoh compatibility plugin for the Magento Hyvä theme provides Tailwind-styled, Alpine-driven templates for the [Magmodules Kiyoh Reviews](https://www.magmodules.eu/magento2-kiyoh-reviews.html) module, so the review page and every review widget render natively on a Hyvä storefront.

The Kiyoh compatibility plugin has the following requirements:
- [Magento 2.4.x](https://github.com/magento/magento2)
- [Hyvä Theme](https://github.com/hyva-themes) 1.x, up to and including the Tailwind 4 builds of 1.5 and later
- [Magmodules Kiyoh Reviews](https://www.magmodules.eu/magento2-kiyoh-reviews.html) 1.12.0 or later

![kiyoh-page](https://github.com/user-attachments/assets/d693262a-6d70-45a2-8313-21544869c9dc)

## What this plugin covers

The Kiyoh module ships its storefront as Luma templates with Knockout and LESS. Hyvä renders neither, so without this plugin the review page shows a loader that never ends and the widgets show their content without any styling. This plugin replaces those templates with Hyvä equivalents:

- **Review page** (`/kiyoh`): header with score and stars, the review list with the one-liner, opinion and recommendation per review, pagination, and the filter modal for rating and year. Built with Alpine.js on the same data the Luma page uses.
- **Review widgets**: Full, Small, Plain, Overview, Textual, Badge, Carousel, Sidebar and Floating.
- **Review sliders**: Default, Extended and Full width.

Settings, imports, invitations, product reviews and structured data stay in the Kiyoh module; this plugin only changes how the storefront is drawn. The Widget Preview page from the Kiyoh configuration (Stores → Configuration → Magmodules → Kiyoh → Widget Preview) shows every widget at once on a Hyvä store view, which is the quickest way to check a theme against all of them.

## Installation

1. Install the module using composer:

```bash
composer require magmodules/magento2-hyva-kiyoh
```

2. Enable the module:

```bash
bin/magento module:enable Magmodules_HyvaKiyOhSR
```

3. Upgrade the database:

```bash
bin/magento setup:upgrade
```

4. Let Hyvä know about the new module:

```bash
bin/magento hyva:config:generate
```

5. Generate the CSS files:

```bash
npm --prefix vendor/hyva-themes/magento2-default-theme/web/tailwind/ run ci
npm --prefix vendor/hyva-themes/magento2-default-theme/web/tailwind/ run build-prod
```

Or from your theme:

```bash
npm --prefix app/design/frontend/<Vendor>/<Theme>/web/tailwind run ci
npm --prefix app/design/frontend/<Vendor>/<Theme>/web/tailwind run build-prod
```

Hyvä 1.5 and later build with Tailwind 4 and read the plugin's `module.css`; earlier versions read its `tailwind.config.js`. Both files ship, so the steps above are the same on every version.

## Upgrading

After updating this plugin or the Kiyoh module, run `bin/magento hyva:config:generate` and rebuild the CSS (step 5) again: the templates carry their Tailwind classes, and a class that was not in the build is not in the stylesheet.

## Magento Support

If you have any questions, please fill out our secure contact form by clicking [here](https://www.magmodules.eu/support-form.html).

## Magmodules & Hyvä

Magmodules and Hyvä have established a strong partnership, working closely together to provide enhanced e-commerce solutions. As an official Hyvä partner, we specialize in developing integrations for various platforms and services.

We have created integrations for well-known providers such as Mollie, Sooqr, Paazl, and many more. This collaboration ensures seamless compatibility and optimized performance for online stores utilizing the Hyvä theme.

## Check out our other Hyvä plugins

- [Magento 2 Hyvä Shopreview](https://github.com/magmodules/magento2-shopreview-hyva)
- [Magento 2 Hyvä Product Review Reminder](https://github.com/magmodules/magento2-reviewreminder-hyva)
- [Magento 2 Hyvä Feedback Company](https://github.com/magmodules/magento2-feedbackcompany-hyva)
- [Magento 2 Hyvä WebwinkelKeur](https://github.com/magmodules/magento2-webwinkelkeur-hyva)
- [Magento 2 Hyvä Google Reviews](https://github.com/magmodules/magento2-googlereviews-hyva)
