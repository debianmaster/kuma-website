---
title: Blue-green Deployment with Kuma in Standalone
content_type: tutorial
---

This tutorial will help you learn how to set up a blue-green deployment for your applications by using {{site.mesh_product_name}} and Flagger as an example.

Tutorials should include an introduction paragraph here. Good introductions explain who this tutorial is for and what this tutorial will help the user accomplish and learn. For example, if you were writing a tutorial about how to get started with a software product, your tutorial could include information about a general overview of what steps the user would be going through, what this software will help them accomplish, and that the end result of this tutorial will be that the software is installed with the basic settings configured. 

## Task section <!-- Header optional if there's only one task section in the article -->

A tutorial section title directs the user to perform an action and generally starts with a verb. For example, "Install the software" or "Configure basic settings".

Each task section should include an introduction paragraph that explains what step the user doing, a brief explanation of the feature, and why the user is completing this step.

### Instructions

Steps in each section should break down the tasks the user will complete in sequential order.

Continuing the previous example of installing software, here's an example:

1. Install `kumactl`:
    ```sh
    curl -L https://kuma.io/installer.sh | sh -
    ```

1. Add the `kumactl` executable to your path.

1. Deploy the control plane:
    ```sh
    kumactl install control-plane --license-path=license.json | kubectl apply -f -
    ```

1. Configure observability with Prometheus:
    ```sh
    kumactl install observability --namespace=kuma-metrics | kubectl apply   -f -
    ```

You can also use tabs in a section. For example, if you can install the software with macOS or Docker, you might have a tab with instructions for macOS and a tab with instructions for Docker.

{% navtabs %}
{% navtab macOS %}

1. Open Terminal...
1. Run....

{% endnavtab %}
{% navtab Docker %}

1. Open Docker...
1. Run....

{% endnavtab %}
{% endnavtabs %}

### Explanation of instructions <!-- Optional, but recommended -->

This section should contain a brief, 2-3 sentence paragraph that summarizes what the user accomplished in these steps and what the outcome was. For example, "The software is now installed on your computer. You can't use it yet because the settings haven't been configured. In the next section, you will configure the basic settings so you can start using the software." 

{:.note}
> **Note**: You can also use notes to highlight important information. Try to keep them short.
## Second task section <!-- Optional -->

Adding additional sections can be helpful if you have to switch from working in one product to another or if you switch from one task, like installing to configuring. 

### Instructions

1. First step.
1. Second step.

### Explanation of instructions <!-- Optional, but recommended -->

## See also <!-- Optional, but recommended -->

This section should include a list of tutorials or other pages that a user can visit to extend their learning from this tutorial.

See the following examples of tutorial documentation:
* [Get started with services and routes](https://docs.konghq.com/gateway/latest/get-started/services-and-routes/)
* [Migrate from OSS to Enterprise](https://docs.konghq.com/gateway/latest/migrate-ce-to-ke/)
* [Set up Vitals with InfluxDB](https://docs.konghq.com/gateway/latest/kong-enterprise/analytics/influx-strategy/)