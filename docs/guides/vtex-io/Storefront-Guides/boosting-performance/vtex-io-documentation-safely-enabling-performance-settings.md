---
title: "Safely enabling performance settings"
slug: "vtex-io-documentation-safely-enabling-performance-settings"
hidden: false
createdAt: "2020-11-11T12:55:23.952Z"
updatedAt: "2022-12-13T20:17:44.058Z"
---
We understand that site performance is a common concern among ecommerce stores since it directly impacts the number of visited pages, sales conversion rate, user session time, bounce rate, and more.

In the following step-by-step, you will learn how to test and implement our [recommendations for optimizing your store's performance](https://developers.vtex.com/docs/guides/vtex-io-documentation-best-practices-for-optimizing-performance).

## Instructions

## Step 1: Applying changes on a production workspace

1. Using the terminal and the [VTEX IO CLI](https://developers.vtex.com/docs/guides/vtex-io-documentation-vtex-io-cli-installation-and-command-reference/), log in to the desired account by running `vtex login {account}`.
2. Run the command `vtex use {productionWorkspace}` to create and use a new [Production workspace](https://developers.vtex.com/docs/guides/vtex-io-documentation-workspace/).
    >⚠️ Remember to replace the values between the curly braces according to your scenario.
3. Using your browser, access the account's admin relative to that workspace.
4. From the account's admin panel, go to *Store Settings > Storefront > Store > Advanced*.
5. Now, considering our documentation on [Best practices for optimizing performance](https://developers.vtex.com/docs/guides/vtex-io-documentation-best-practices-for-optimizing-performance), activate the desired features, and save the changes.
6. Access your store in the current workspace that you're working in and check if the performance improvements were applied.

> ℹ️ Note that it might take some time before changes are applied.

## Step 2: Testing and analyzing performance

1. Review and test all the main pages of your store, making sure that the changes didn't cause any side effects, such as style inconsistencies or undesired behaviors.
2. Access [Google PageSpeed Insights.](https://developers.google.com/speed/pagespeed/insights)
3. Using the following URL pattern: `https://{account}.myvtex.com/?workspace={productionWorkspace}`, check your store's performance in the production workspace you're currently working.

>⚠️ Using the standard URL pattern `https://{workspace}--{account}.myvtex.com/` won't show the performance score of your store in the specified workspace. Thus, keep in mind: to analyze performance in a workspace, **you must use the `?workspace={productionWorkspace}` query string** as shown in Step 2.3.

## Step 3: Making your changes publicly available

If you're happy with your changes, run `vtex promote` to promote your workspace and benefit from a faster store.

> ℹ️ Before promoting your workspace to master, we recommend that you measure the performance improvements by comparing the performance score in the production and the master workspace.
