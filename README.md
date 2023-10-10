
![image](https://github.com/magmodules/magento2-kiyoh-hyva/assets/24823946/f2baee4a-b8f4-4d84-82d7-54b5ac8e0649)


# Kiyoh Hyvä Compatibility plugin

The Kiyoh plugin for Magento is a powerful integration that seamlessly connects your Magento store with the renowned review platform, Kiyoh. This plugin offers comprehensive functionality to enhance your online store's reputation management and streamline the customer feedback process. With its compatibility with the Hyva theme, the plugin ensures a smooth and seamless user experience while incorporating the robust features of the Kiyoh platform. By leveraging the Kiyoh plugin, you can effectively collect and manage customer reviews, ratings, and testimonials, building trust with potential customers and enhancing your brand reputation. With advanced features like automatic review requests, customizable widgets, and rich snippet integration, the Kiyoh plugin empowers you to actively engage with customers, gather valuable feedback, and optimize your online store's performance.

Kiyoh plugin Hyvä Compatibility plugin for the Magento Hyva theme has the following requirements:
- [Magento 2.4.+](https://github.com/magento/magento2)
- [Hyvä](https://github.com/hyva-themes)
- [Magmodules Kiyoh Reviews](https://www.magmodules.eu/magento2-kiyoh-reviews.html)    


<img width="946" alt="kiyoh-hyva-magento" src="https://github.com/magmodules/magento2-kiyoh-hyva/assets/24823946/88e1d1c3-c66b-499d-a12e-956296dc4217">


## About Kiyoh Plugin

The Kiyoh plugin for Magento is a robust integration that seamlessly connects your Magento store with the renowned review platform, Kiyoh. This plugin offers a comprehensive set of features to enhance your online store's reputation management and streamline the customer feedback process.

By integrating the Kiyoh plugin into your Magento store, you can effortlessly incorporate the powerful review platform while ensuring compatibility with the Hyva theme. This guarantees a consistent and visually appealing user experience across your website.

With the Kiyoh plugin, you gain the ability to effectively manage your online store's reputation by collecting and showcasing customer reviews, ratings, and testimonials. By leveraging the power of social proof, you can build trust with potential customers and enhance the reputation of your brand.

The plugin provides essential tools for review management, allowing you to moderate and manage reviews conveniently within your Magento admin panel. You have full control over the display of reviews on your website, ensuring that only relevant and valuable feedback is visible to your customers.

Additionally, the Kiyoh plugin offers advanced features such as automatic review requests, email notifications, customizable review widgets, and rich snippet integration for improved search engine optimization (SEO). These features empower you to actively engage with your customers, gather valuable feedback, and elevate the overall shopping experience on your Magento store.

In conclusion, the Kiyoh plugin for Magento, with its compatibility with the Hyva theme, offers a powerful solution for seamlessly integrating the Kiyoh review platform into your online store. It enables you to effectively manage your store's reputation, collect valuable customer feedback, and foster trust with your audience.
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
php bin/magento hyva:config:generate
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

## Kiyoh Magento plugin features

- Seamless integration
- Review collection automation
- Customizable review widgets
- Rich snippet integration
- Hyvä Compatibility
- Host it all on your platform


## Magento Support

If you have any questions, please fill out our secure contact form by clicking [here](https://www.magmodules.eu/support-form.html).

## Magmodules & Hyva

Magmodules and Hyva have established a strong partnership, working closely together to provide enhanced e-commerce solutions. As an official Hyva partner, we specializes in developing integrations for various platforms and services. 

We have created integrations for well-known providers such as Mollie, Sooqr, Paazl, and many more. This collaboration ensures seamless compatibility and optimized performance for online stores utilizing the Hyva theme. Through our partnership, Magmodules and Hyva strive to deliver comprehensive and tailored solutions to meet the diverse needs of e-commerce businesses.



## Checkout our other Hyva Plugins!

[- Magento 2 Hyvä Shopreview](#) 
 
[- Magento 2 Hyvä Product Review Reminder](#) 

[- Magento 2 Hyvä Mollie React Checkout](#) 

[- Magento 2 Hyvä Checkout](#) 

[- Magento 2 Hyvä Mollie React Checkout](#) 

[- Magento 2 Hyvä Paazl](#) 
