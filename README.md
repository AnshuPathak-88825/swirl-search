[![Swirl](https://github.com/swirlai/swirl-search/wiki/images/hack_swirl_fest.png)](https://join.slack.com/t/swirlmetasearch/shared_invite/zt-1qk7q02eo-kpqFAbiZJGOdqgYVvR1sfw)

<div align="center">

[![Swirl](https://github.com/swirlai/swirl-search/wiki/images/transparent_header_3.png)](https://www.swirl.today)

</div>

<h1 align="center">Swirl</h1>

<div align="center">

### Swirl is open-source software that simultaneously searches multiple content sources and returns AI ranked results.

<div align="center">


[𝚂𝚝𝚊𝚛𝚝 𝚂𝚎𝚊𝚛𝚌𝚑𝚒𝚗𝚐](#-try-swirl-now-in-docker) ⦁
[𝚂𝚕𝚊𝚌𝚔](https://join.slack.com/t/swirlmetasearch/shared_invite/zt-1qk7q02eo-kpqFAbiZJGOdqgYVvR1sfw) ⦁
[𝙺𝚎𝚢 𝙵𝚎𝚊𝚝𝚞𝚛𝚎𝚜 ](#-key-features) ⦁
[𝙲𝚘𝚗𝚝𝚛𝚒𝚋𝚞𝚝𝚎](#-contributing-to-swirl) ⦁
[𝙳𝚘𝚌𝚞𝚖𝚎𝚗𝚝𝚊𝚝𝚒𝚘𝚗](#-documentation) ⦁ [𝙲𝚘𝚗𝚗𝚎𝚌𝚝𝚘𝚛𝚜](#-list-of-connectors)


</div>

---

<br/>

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg?color=088395&logoColor=blue&style=flat-square)](https://opensource.org/license/apache-2-0/)
[![GitHub Release](https://img.shields.io/github/v/release/swirlai/swirl-search?style=flat-square&color=8DDFCB&label=Release)](https://github.com/swirlai/swirl-search/releases)
[![Slack](https://custom-icon-badges.demolab.com/badge/Join%20Our%20Slack-black?style=flat-square&logo=slack&color=0E21A0&logoColor=white)](https://join.slack.com/t/swirlmetasearch/shared_invite/zt-1qk7q02eo-kpqFAbiZJGOdqgYVvR1sfw)
[![PRs Welcome](https://custom-icon-badges.demolab.com/badge/PRs%20Welcome-black?style=flat-square&logo=github&color=4D2DB7&logoColor=C70039)](#contributing-to-swirl)
[![Website](https://custom-icon-badges.demolab.com/badge/www.swirl.today-black?style=flat-square&logo=globe&color=241468&logoColor=white)](https://www.swirl.today)
[![Docker Build](https://github.com/swirlai/swirl-search/actions/workflows/docker-image.yml/badge.svg?style=flat-square&branch=main)](https://github.com/swirlai/swirl-search/actions/workflows/docker-image.yml)
[![Tests](https://github.com/swirlai/swirl-search/actions/workflows/smoke-tests.yml/badge.svg?branch=main)](https://github.com/swirlai/swirl-search/actions/workflows/smoke-tests.yml)

</div>

Swirl is open source software that simultaneously searches multiple content sources and returns AI ranked results. Prompt your choice of Generative AI using the top N results to get answers incorporating your own data.

Swirl can connect to:

* Databases (SQL & NoSQL, Google BigQuery)
* Public data services (Google Programmable Search, Arxiv.org, etc.)
* Enterprise sources (Microsoft 365, Jira, Miro etc.)

And generate insights with AI and LLMs like ChatGPT. Start discovering and generating the answers you need based on your data.

Swirl is as simple as ABC: (a) Download YML, (b) Start in Docker, (c) Search with Swirl. From there, add credentials to preloaded SearchProviders to get results from more sources.

## 🚀 Try Swirl with ChatGPT 

![Swirl with ChatGPT as a configured AI Model](https://github.com/swirlai/swirl-search/wiki/images/Animation_1.gif)

_Swirl with ChatGPT as a configured AI Model._

>**Note**
> We need your help 🙏. Help us create more examples of things you can or want to do with Swirl. Join our [Slack Community](https://join.slack.com/t/swirlmetasearch/shared_invite/zt-1qk7q02eo-kpqFAbiZJGOdqgYVvR1sfw) to discuss and learn more. We'd be very happy to help you contribute 🤗!

<br/>

# 🔎 How Swirl Works

Swirl adapts and distributes user queries to anything with a search API - search engines, databases, noSQL engines, cloud/SaaS services, data siloes, etc. And uses Large Language Models to re-rank the unified results *without* extracting or indexing *anything*. 

![Swirl Diagram](https://github.com/swirlai/swirl-search/wiki/images/Animation_2.gif)

<br/>

# 🔌 List of Connectors

<img src="https://github.com/swirlai/swirl-search/wiki/images/Connectors_2.png" height=60% width=70%/>

➕ **For Enterprise Support on Connectors**  Contact the Swirl Team at: [support@swirl.today](mailto:support@swirl.today)  

🚀 **Help Us Expand!** Want to see a new connector? [Contribute by adding a connector](#👩‍💻-contributing-to-swirl) and join our growing community of contributors. 

<br/>

# Installation and Setup

### Step 1: Clone the Repository

Begin by cloning the Swirl repository from GitHub:

```bash
git clone repo-link
cd swirl-search
```

### Step 2: Set Up Microsoft 365 Credentials
Before proceeding, you need to set up [Microsoft 365 (M365)](https://docs.swirl.today/4.-M365-Guide.html) credentials. Refer to the M365 Guide for detailed instructions on how to obtain these credentials.

Complete the '.env.dist' file in the project's root directory and add the M365 credentials as follows:
```bash
MICROSOFT_CLIENT_ID='your-microsoft-client-id'
MICROSOFT_CLIENT_SECRET='your-microsoft-client-secret'
MICROSOFT_REDIRECT_URI='your-microsoft-redirect-uri'
```
After a few minutes, the Swirl application should be up and running.
### Step 3: Build and Run Swirl
With the M365 credentials in place, you can now build and run Swirl using Docker:
### Prerequisites
- To run Swirl in Docker, you must have the latest Docker app for MacOS, Linux, or Windows installed and running locally.

- Windows users must also install and configure either the WSL 2 or the Hyper-V backend, as outlined in the System Requirements for installing Docker Desktop on Windows.

## Start Swirl in Docker
> **Warning** 
> Make sure the Docker app is running before proceeding

Download the Docker Compose configuration file:
bash
Copy code
```
curl https://raw.githubusercontent.com/swirlai/swirl-search/main/docker-compose.yaml -o docker-compose.yaml
```
In MacOS or Linux, run the following command from the Console:
bash
Copy code
```
docker-compose pull && docker-compose up
```
In Windows, run the following command from PowerShell:
bash
Copy code
docker 

```
compose up

```

## Step 4: Access Swirl

- 🌐 After running the above commands, open your web browser and navigate to [http://localhost:8000](http://localhost:8000).

- 🎉 Congratulations! You've successfully set up the Swirl project. You can now start using Swirl for metasearch and exploration.

- 👤 You'll be directed to the sign-in page. To access Swirl, use the following credentials:

   - Username: admin
   - Password: password

- 🔒 If the search page appears, click Log Out at the top right. The Swirl login page will appear.

- 🔍 Enter a search in the search box and press the Search button. Ranked results appear in just a few seconds.

Feel free to explore the project's documentation for further information and features.

If you encounter any issues or have questions, please refer to our [Slack support channel](https://join.slack.com/t/swirlmetasearch/shared_invite/zt-1qk7q02eo-kpqFAbiZJGOdqgYVvR1sfw) for assistance.

## Next Steps 👇

* Check out the details of our [latest release](https://github.com/swirlai/swirl-search/releases)!

* Head over to the [Quick Start Guide](https://github.com/swirlai/swirl-search/wiki/1.-Quick-Start) and install Swirl locally!

<br/>

# 🌟 Key Features

| ✦ | Feature |
|:-----:|:--------|
| 📌 | [Microsoft 365 integration and OAUTH2 support](https://github.com/swirlai/swirl-search/wiki/4.-M365-Guide) |
| 🔍 | [SearchProvider configurations](https://github.com/swirlai/swirl-search/tree/main/SearchProviders) for all included Connectors. They can be [organized with the active, default and tags properties](https://github.com/swirlai/swirl-search/wiki/2.-User-Guide#organizing-searchproviders-with-active-default-and-tags). |
| ✏️ | [Adaptation of the query for each provider](https://github.com/swirlai/swirl-search/wiki/2.-User-Guide#search-syntax) such as rewriting `NOT term` to `-term`, removing NOTted terms from providers that don't support NOT, and passing down the AND, + and OR operators. |
| ⏳ | [Synchronous or asynchronous search federation](https://github.com/swirlai/swirl-search/wiki/5.-Developer-Guide#architecture) via [APIs](http://localhost:8000/swirl/swagger-ui/) |
| 🛎️ | [Optional subscribe feature](https://github.com/swirlai/swirl-search/wiki/5.-Developer-Guide#subscribe-to-a-search) to continuously monitor any search for new results |
| 🛠️ | Pipelining of [Processor](https://github.com/swirlai/swirl-search/wiki/5.-Developer-Guide#develop-new-processors) stages for real-time adaptation and transformation of queries, responses and results |
| 🗄️ | [Results stored](https://github.com/swirlai/swirl-search/wiki/6.-Developer-Reference#result-objects) in SQLite3 or PostgreSQL for post-processing, consumption and/or analytics |
| ➡️ | Built-in [Query Transformation](https://github.com/swirlai/swirl-search/wiki/5.-Developer-Guide#using-query-transformations) support, including re-writing and replacement |
| 📖 | [Matching on word stems](https://github.com/swirlai/swirl-search/wiki/6.-Developer-Reference#cosinerelevancypostresultprocessor) and [handling of stopwords](https://github.com/swirlai/swirl-search/wiki/5.-Developer-Guide#configure-stopwords-language) via NLTK |
| 🚫 | [Duplicate detection](https://github.com/swirlai/swirl-search/wiki/5.-Developer-Guide#detect-and-remove-duplicate-results) on field or by configurable Cosine Similarity threshold |
| 🔄 | Re-ranking of unified results [using Cosine Vector Similarity](https://github.com/swirlai/swirl-search/wiki/6.-Developer-Reference#cosinerelevancypostresultprocessor) based on [spaCy](https://spacy.io/)'s large language model and [NLTK](https://www.nltk.org/) |
| 🎚️ | [Result mixers](https://github.com/swirlai/swirl-search/wiki/6.-Developer-Reference#mixers-1) order results by relevancy, date or round-robin (stack) format, with optional filtering of just new items in subscribe mode |
| 📄 | Page through all results requested, re-run, re-score and update searches using URLs provided with each result set |
| 📁 | [Sample data sets](https://github.com/swirlai/swirl-search/tree/main/Data) for use with SQLite3 and PostgreSQL |
| ✒️ | [Optional spell correction](https://github.com/swirlai/swirl-search/wiki/5.-Developer-Guide#add-spelling-correction) using [TextBlob](https://textblob.readthedocs.io/en/dev/quickstart.html#spelling-correction) |
| ⌛ | [Optional search/result expiration service](https://github.com/swirlai/swirl-search/wiki/3.-Admin-Guide#search-expiration-service) to limit storage use |
| 🔌 | Easily extensible [Connector](https://github.com/swirlai/swirl-search/tree/main/swirl/connectors) and [Mixer](https://github.com/swirlai/swirl-search/tree/main/swirl/mixers) objects |


<br/>

# 👩‍💻 Contributing to Swirl 

**Got a brilliant idea or improvement for Swirl?** We're all ears—and thrilled you're here to help!

🔗 **Get Started in 3 Easy Steps**:
1. **Connect with Fellow Enthusiasts** - Jump into our [Slack community](https://join.slack.com/t/swirlmetasearch/shared_invite/zt-1qk7q02eo-kpqFAbiZJGOdqgYVvR1sfw) and share your ideas. You'll find a welcoming group of Swirl enthusiasts and team members eager to assist and collaborate.
2. **Branch It Out** - Always branch off from the `develop` branch with a descriptive name that encapsulates your idea or fix. Remember, all PRs should be made to the `develop` branch to ensure `main` remains our stable gold-standard.
3. **Start Your Contribution** - Ready to get your hands dirty? Make sure all contributions come through a GitHub pull request. We roughly follow the [Gitflow branching model](https://nvie.com/posts/a-successful-git-branching-model/), so all changes destined for the next release should be made to the `develop` branch.

📚 **First time contributing on GitHub?** No worries, the [GitHub documentation](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) has you covered with a great guide on contributing to projects.

💡 Every contribution, big or small, makes a difference. Join us in shaping the future of Swirl!


<br/>

# ☁ Use the Swirl Cloud 

For information about Swirl as a managed service, please [contact us](mailto:hello@swirl.today)!

<br/>

# 📖 Documentation

[Home](https://github.com/swirlai/swirl-search/wiki) | [Quick Start](https://github.com/swirlai/swirl-search/wiki/1.-Quick-Start) | [User Guide](https://github.com/swirlai/swirl-search/wiki/2.-User-Guide) | [Admin Guide](https://github.com/swirlai/swirl-search/wiki/3.-Admin-Guide) | [M365 Guide](https://github.com/swirlai/swirl-search/wiki/4.-M365-Guide) | [Developer Guide](https://github.com/swirlai/swirl-search/wiki/5.-Developer-Guide) | [Developer Reference](https://github.com/swirlai/swirl-search/wiki/6.-Developer-Reference)

<br/>

# 👷‍♂️ Need Help? We're Here for You!

At Swirl, every user matters to us. Whether you're a beginner finding your way or an expert with feedback, we're here to support, listen, and help. Don't hesitate to reach out us.

* 🎉 **Join the Conversation:** Dive into our vibrant [Swirl Metasearch Community on Slack](https://join.slack.com/t/swirlmetasearch/shared_invite/zt-1qk7q02eo-kpqFAbiZJGOdqgYVvR1sfw) - it's where all the magic happens!

* 📧 **Direct Support:** For any questions, suggestions, or even a simple hello, drop us an email at [support@swirl.today](mailto:support@swirl.today). We cherish every message and promise to get back to you promptly!

* 💼 **Request A Connector (Enterprise Support)** Want to see a new connector quickly and fast. Contact the Swirl Team at: [support@swirl.today](mailto:support@swirl.today)

Remember, you're part of our family now. 🌍💙


<br/>
# Swirl Project Setup Guide

Welcome to Swirl, a powerful metasearch and exploration tool. This guide will walk you through the installation and setup process.
