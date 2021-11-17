---
title: FAQ
layout: default
---

## {{ page.title }}
{: .page-header .no_toc}

*These FAQs primarily target developers working on publishing a dataset. Don't see your question listed below? Please contact [David M. Rogers](mailto:rogersdm@ornl.gov).*

* Table of Contents
{:toc}

### How do I set up a GitHub account?

If you’re new to GitHub and open source in general, figuring out how to get set up can be a challenge. You may want to read through the GitHub Help pages on [setting up and managing your GitHub profile](https://help.github.com/categories/setting-up-and-managing-your-github-profile/).

1. [Create an account on GitHub](https://github.com/join).

    You *do not need* a separate work account and personal account. Instead, you can [link multiple email addresses to the same GitHub account](https://help.github.com/articles/adding-an-email-address-to-your-github-account/), which is almost always preferred.

2. [Update your profile information](https://github.com/settings/profile).

    * **Photo**: A headshot photo, or image that is uniquely you.
    * **Name**: Your first and last name.
    * **Bio**: Include a few words about yourself! Don't forget to mention @ORNL.
    * **URL**: This might be your [people.llnl.gov](https://people.llnl.gov) page, or a personal website if you prefer.
    * **Company**: Probably `Oak Ridge National Laboratory, @ORNL`.
    * **Location**: Your primary location.

3. Add your `@ORNL` email address (and any aliases) to your [Email Settings](https://github.com/settings/emails) page. This will link any commits done via [your Git identity](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup#Your-Identity) to your GitHub account.

4. [Enable two-factor authentication (2FA)](https://github.com/settings/security).

### What is two-factor authentication (2FA)?

There are several options for configuring 2FA for your GitHub account:

* [YubiKey](https://yubico.com) hardware security keys
    * YubiKeys are the preferred 2FA option, due to the security of the YubiKey hardware tokens. If you have been issued an ORNL YubiKey, it is highly recommended for securing your GitHub (and other) accounts which support them.
    * [Learn more about setting up your YubiKey with GitHub.com](https://help.github.com/articles/configuring-two-factor-authentication/#configuring-two-factor-authentication-using-fido-u2f)

* [Google Authenticator](https://support.google.com/accounts/answer/1066447)
    * Google Authenticator is a mobile application which you can install on your personal or government issued phone.
    * It provides a one-time token (OTP) which you can use to authenticate to GitHub.com
    * [Learn more about setting up Google Authenticator with GitHub.com](https://help.github.com/articles/configuring-two-factor-authentication/#configuring-two-factor-authentication-using-a-totp-mobile-app)
    
* [Authy](https://authy.com/guides/github/)
    * Authy is a desktop- or laptop-based application which can be used to generate a one-time token (OTP) for use logging in to GitHub.com.
    * This option is usually best for when you do all or most of your work in an environment where you do not have access to a mobile phone or USB YubiKey.
    * [Learn more about setting up Authy with GitHub.com](https://authy.com/guides/github/)

Additional 2FA info:
    
* You also have the option during 2FA to generate and save a list of recovery codes to get into your account in the event you lose access to one of your 2FA methods. This is *highly* recommended, and the recovery codes should be stored someplace safe. Some options for storing your recovery codes include:
    * Printing the codes and storing them in a safe place in your office.
    * Storing the recovery codes in a password manager that you might be using.
    
* We recommend that you set up *MULTIPLE* 2FA options. This can protect your access to your account in the event that you lose access to one of your authenticators.
    * For more information, check out the [Two-factor Authentication](https://github.com/blog/1614-two-factor-authentication) post on the GitHub Blog.
    * Having trouble setting up 2FA? Contact the [LLNL GitHub admins](mailto:github-admin@llnl.gov) who may be able to help.

### How do I get my dataset reviewed and released for GitHub?

Create your repository and dataset on its own.  Both [code.ornl.gov](https://code.ornl.gov) and github are good options.
Next, send an email to this site's maintainer to get information
on the review process and add its listing here.


### What is/isn’t allowed to be included in my repo?

Remember that these repositories *are hosted* on GitHub servers, *NOT LLNL servers*, and content placed in them should be limited to "email like" communications. That means:

* NO Classified
* NO Export Controlled
* NO Official Use Only (OUO)
* NO Health Insurance Portability and Accountability Act (HIPAA)
* NO Personally Identifiable Information (PII)
* NO NDA or vendor-proprietary information
* NO Unclassified Controlled Information (UCI)
* NO Unclassified Controlled Nuclear Information (UCNI)

When in doubt, contact a Derivative Classifier (DC) for further guidance.


### My project is approved for release. Now what?

Make sure your repo follows best practices and includes the following informational files:

* An appropriate open source **license**. Details and examples can be seen at [LLNL Software Licensing](https://software.llnl.gov/about/licenses).

* A [**README**](https://guides.github.com/features/wikis/) file that summarizes what the software does and how others can use and contribute to it.

* A **NOTICE** containing any required funding acknowledgments for your project.

After your project has been initially released on GitHub and you are ready to provide a new version, a good practice is to tag the version and include [**release notes**](https://github.com/LLNL/.github/blob/main/community-health/release-template.md).

Another good practice is to provide **user documentation**. Read the Docs (RtD) is a common platform for user guides, tutorials, quick start instructions, and other forms of documentation.

Submit your repo to [**DOE CODE**](https://www.osti.gov/doecode/faq#what-is) so others can find it when searching through DOE-funded projects. After your repo is included in DOE CODE, you may also want to add the **digital object identifier** (DOI) to the repo.

If your repo is research software, consider submitting it to a journal that publishes scientific datasets.


### How does this website’s catalog work?

* The [`input_lists.json` file](https://github.com/frobnitzem/olcf-datasets/blob/main/_datasets/input_lists.json) lists information on included repositories.

* If you have a project logo, please follow the [instructions](https://github.com/frobnitzem/olcf-datasets/tree/main/assets/images/logos) for naming and uploading the file.


### How do I contribute to a dataset?

Refer to individual projects for their requirements on accepting contributions. In general though, we follow the "fork and pull" Git workflow model:

1. Fork a repository.

2. Develop your changes in your fork.

3. Sync your fork to the upstream repository (`git remote add upstream git@github.com:org/repo.git`).

4. Create a pull request to the "upstream" repository.

5. If approved, changes will be merged in by a repository maintainer.
