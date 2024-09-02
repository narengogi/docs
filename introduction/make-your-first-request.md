---
description: Integrate Portkey and analyze your first LLM call in 2 minutes!
---

# Make Your First Request

## 1. Get your Portkey API Key

[Create](https://app.portkey.ai/signup) or [log in](https://app.portkey.ai/login) to your Portkey account. Grab your account's API key from the "Settings" page.

<div align="left" data-full-width="false">

<figure><img src="../.gitbook/assets/CleanShot 2024-08-14 at 02.35.03.gif" alt=""><figcaption><p>Copy your Portkey account API key</p></figcaption></figure>

</div>

Based on your access level, you might see the relevant permissions on the API key modal - tick the ones you'd like, name your API key, and save it.

## 2. Integrate Portkey

Portkey offers a variety of integration options, including SDKs, REST APIs, and native connections with platforms like OpenAI, Langchain, and LlamaIndex, among others.

### Through the OpenAI SDK

If you're using the **OpenAI SDK**, import the Portkey SDK and configure it within your OpenAI client object:

{% content-ref url="../integrations/llms/openai/" %}
[openai](../integrations/llms/openai/)
{% endcontent-ref %}

### Portkey SDK

You can also use the **Portkey SDK / REST APIs** directly to make the chat completion calls. This is a more versatile way to make LLM calls across any provider:

{% content-ref url="../api-reference/portkey-sdk-client.md" %}
[portkey-sdk-client.md](../api-reference/portkey-sdk-client.md)
{% endcontent-ref %}

Once, the integration is ready, you can view the requests reflect on your Portkey dashboard.

<figure><img src="../.gitbook/assets/analytics_logs (1).gif" alt=""><figcaption></figcaption></figure>

### Other Integration Guides

<table data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td><strong>Azure OpenAI</strong></td><td><a href="../integrations/llms/azure-openai.md">azure-openai.md</a></td></tr><tr><td><strong>Anthropic</strong></td><td><a href="../integrations/llms/anthropic.md">anthropic.md</a></td></tr><tr><td><strong>Langchain</strong></td><td><a href="../integrations/libraries/langchain-python.md">langchain-python.md</a></td></tr><tr><td><strong>LlamaIndex</strong></td><td><a href="../integrations/libraries/llama-index-python.md">llama-index-python.md</a></td></tr><tr><td><strong>Ollama</strong></td><td><a href="../integrations/llms/ollama.md">ollama.md</a></td></tr><tr><td><strong>Others</strong></td><td><a href="../provider-endpoints/gateway-for-other-apis.md">gateway-for-other-apis.md</a></td></tr></tbody></table>

## 3. Next Steps

Now that you're up and running with Portkey, you can dive into the various Portkey features to learn about all of the supported functionalities:

<table data-view="cards"><thead><tr><th></th><th data-hidden data-type="content-ref"></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td>Observability</td><td><a href="../product/observability/">observability</a></td><td></td></tr><tr><td>AI Gateway</td><td></td><td><a href="../product/ai-gateway/">ai-gateway</a></td></tr><tr><td>Prompt Library</td><td></td><td><a href="../product/prompt-library.md">prompt-library.md</a></td></tr><tr><td>Autonomous Fine-Tuning</td><td></td><td><a href="../product/autonomous-fine-tuning.md">autonomous-fine-tuning.md</a></td></tr></tbody></table>

***

{% hint style="success" %}
While you're here, why not [give us a star](https://git.new/ai-gateway-docs)? It helps us a lot!
{% endhint %}

## FAQs

### Will Portkey increase the latency of my API requests?

Portkey is hosted on edge workers throughout the world and our servers ensure the least latency roundtrips. Our benchmarks estimate a total latency addition between 20-40ms.

Our edge worker locations:

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="" width="375"><figcaption></figcaption></figure>

### Is my data secure?

Portkey is ISO:27001 and SOC 2 certified. We're also GDPR compliant. This is proof that we maintain the best practices involving security of our services, data storage and retrieval. All your data is encrypted in transit and at rest.

If you're still worried about your data passing through Portkey, we recommend one of the below options:

1. On request, we can enable a feature that does NOT store any of your request and response body objects in the Portkey datastores or our logs.
2. For enterprises, we offer managed hosting to deploy Portkey inside private clouds.

If you need to talk about these options, feel free to drop us a note on hello@portkey.ai

### Will Portkey scale if my app explodes?

Portkey has been tested to handle millions of requests per second. We serve over 10M requests everyday with a 99.99% uptime. We're built of top of scalable infrastructure and can handle huge loads without breaking a sweat.

[**View our Status Page**](https://status.portkey.ai)

### Does Portkey impose timeouts on requests?

We do not impose **any explicit timeout** for our free OR paid plans currently. In the past, we have had users experience timeouts from various other frameworks, but Portkey does not time out requests on our end.

### Do you support sign ups from non-google/gmail accounts?

Yes! We support registrations with Microsoft accounts - this is currently in beta. Please reach out on support@portkey.ai or [request on Discord](https://discord.gg/kXYKpPGasJ) for access to MS login.

### Where can I reach you?

We're available all the time on [Discord](https://discord.gg/DD7vgKK299), or on our support email - support@portkey.ai