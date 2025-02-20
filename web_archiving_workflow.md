UGA Libraries Web Archiving Workflow
====
July 2019

This workflow provides an overview of the steps involved in web crawling, with links to the[ Archive-It User Guide](https://support.archive-it.org/hc/en-us/categories/201179946-Archive-It-User-Guide) which details how to perform each step. See the [Archive-It Glossary](https://support.archive-it.org/hc/en-us/articles/208111686-Glossary-of-Archive-It-and-Web-Archiving-Terms) for definitions of terms.


# Workflow Overview

1. [Select seeds to crawl](#1-select-seeds-to-crawl)
2. [Obtain permissions](#2-obtain-permissions)
3. [Add seeds to the seed list](#3-add-seeds-to-the-seed-list)
4. [Add seeds to collections](#4-add-seeds-to-collections)
5. [Crawl the seeds](#5-crawl-the-seeds)
6. [Quality assurance](#6-quality-assurance)
7. [Add seed metadata](#7-add-seed-metadata)
8. [Make the seeds public](#8-make-the-seeds-public)
9. [Preservation](#9-preservation)

# Workflow Steps

## 1. Select Seeds to Crawl

*   Do we have a related collection?

*   Is it related to an important collecting area?

*   Is the seed well represented in the Wayback Machine? Even if it is, if it is important to our collections we may crawl it anyway to have a local copy.


## 2. Obtain Permissions

*   If we have an established collecting relationship, no additional permissions are necessary.

*   If not, send a notification to the site owner of our intent to crawl. Allow four weeks for a response. No response will be taken as permission to crawl. You can continue with the rest of the workflow, except for providing public access, during the four weeks. Contact the site owner even if crawling is not restricted by robots.txt as a courtesy and to potentially start a collecting relationship.


## 3. Add Seeds to the Seed List

Each department maintains a separate seed list, typically a spreadsheet, which includes all seeds that have been crawled or are candidates for future crawling.

The seed list and Archive-It reports make up the documentation of the crawl. Researchers sometimes need this information, particularly related to scoping decisions, to understand the completeness of the record.

Information to include:

*   Information about the site (url, creator, related collection, type of site).

*   Reason for collecting.

*   Collecting priority. If the Archive-It quota is getting low, do not crawl lower priority sites unless there is sufficient quota remaining at the end of the subscription year (ends March 14).

*   Permissions information (deed of gift, if notification sent to the site owner).

*   Crawl information ([intended crawl frequency](https://support.archive-it.org/hc/en-us/articles/208333013-Schedule-crawls#Howtoschedulecrawls-Howtoassignacrawlfrequencytoyourseed(s)), result of test crawls).


## 4. Add Seeds to Collections

Seeds are organized into [collections](https://support.archive-it.org/hc/en-us/articles/360000706843-How-seeds-documents-and-collections-work-together) to assist researchers with browsing on the public site and to assist archivists with management activities like [batch scoping](https://support.archive-it.org/hc/en-us/articles/360020571251-Adding-Seed-Level-Scoping-Rules-in-Bulk-) or [batch metadata](https://support.archive-it.org/hc/en-us/articles/208012996-How-to-upload-and-download-metadata).

Collections are primarily organized by topic, but can also be by department or creator. Seeds within collections can be further [organized into groups](https://support.archive-it.org/hc/en-us/articles/208332743-Organize-seeds-as-a-group-).

*   [Make a new collection in Archive-It](https://support.archive-it.org/hc/en-us/articles/207999936-Create-and-manage-a-collection) if needed and [add collection metadata.](https://support.archive-it.org/hc/en-us/articles/360014251692-Add-and-edit-collection-information) Use the [UGA Web Archives Metadata Profile](metadata_profile.md) to determine what information to include.

*   [Add the seeds to a collection.](https://support.archive-it.org/hc/en-us/articles/208331753-Select-Seed-URLs) A seed may only belong to one collection.


## 5. Crawl the Seeds

Seeds may be crawled as test or one-time production crawls ([from the collection's seed list](https://support.archive-it.org/hc/en-us/articles/208001026-Manually-start-test-and-one-time-crawls) or [with InstaCrawl](https://support.archive-it.org/hc/en-us/articles/360013680631-Crawl-new-seeds-immediately-with-InstaCrawl)), or [set on a crawl schedule](https://support.archive-it.org/hc/en-us/articles/208333013-Schedule-crawls).

It is **HIGHLY RECOMMENDED TO USE TEST CRAWLS** as much as possible to responsibility manage our data quota. The first time a site is crawled, a test crawl **MUST** be used. Test crawls do not count against the quota until they are saved but other crawl types do.

To limit accidental capture of data from scheduled crawls, **ALL SCHEDULED CRAWLS MUST USE A DATA LIMIT** instead of a time limit when scheduling the crawl. Also review the capture periodically to see if the limit is being reached and the scope needs to be adjusted to fully capture the site. We have had multiple cases where a website was restructured and a large amount of content we did not want was captured by a scheduled crawl. Archive-It will continue to save this data above our data limit until the schedule crawl finishes, which would make us responsible for paying for the next level of data limit.

*   Each test crawl should include just one seed or a few similar seeds because test crawls must be saved or deleted in their entirety.

*   The standard crawl only captures sites from the seed domain. To capture sites linked from the seed as well, [use a different seed type](https://support.archive-it.org/hc/en-us/articles/208332843-Assign-and-edit-a-seed-type-).

*   Adjust the [scoping rules.](https://support.archive-it.org/hc/en-us/articles/360015086931-Modify-your-collection-or-seed-scope).

    *   Default scoping rules are applied automatically for social media sites. For additional specificity, see [scoping guidance for specific types of sites.](https://support.archive-it.org/hc/en-us/articles/208001336-Scoping-guidance-for-specific-types-of-sites).

    *   You may also need to use [regular expressions](https://support.archive-it.org/hc/en-us/articles/208332963-Modify-crawl-scope-with-a-Regular-Expression) to exclude other languages from Twitter.

    *   Add additional scoping rules to [include](https://support.archive-it.org/hc/en-us/articles/208001106-Expand-the-scope-of-your-crawl) or [exclude](https://support.archive-it.org/hc/en-us/articles/208332933-Limit-your-crawl) parts of the seed site or linked sites.

*   If desired, [only capture PDFs](https://support.archive-it.org/hc/en-us/articles/208332953-Limit-your-crawl-to-archive-only-PDFs).

*   If necessary, [address robots.txt exclusions](https://support.archive-it.org/hc/en-us/articles/208001096-Avoid-robots-txt-exclusions). Add '/robots.txt' to the end of a url to see the site's robots.txt file.

*   [Run a test crawl](https://support.archive-it.org/hc/en-us/articles/208001226-Run-monitor-and-save-a-test-crawl). You can [monitor a crawl as  it runs and cancel it](https://support.archive-it.org/hc/en-us/articles/208332973-Monitor-crawls) with the "Stop Crawl" button if there is a mistake, e.g. the scope is too broad or a one-time production crawl was run instead of a test crawl.


## 6. Quality Assurance

The crawled sites should be viewable via the link in the [seed tab of the crawl report](https://support.archive-it.org/hc/en-us/articles/115001487123-How-can-I-view-my-test-crawl-results-in-Wayback-) approximately 24 hours after the crawl completes.

New crawls should be carefully checked to ensure the right content has been captured. Repeat crawls should be briefly checked in case a change to the site requires the scoping rules be updated.

You have 60 days to review and save a test crawl before the content (but not its crawl reports) are deleted.

*   Confirm the overall total size is about what you expected based on the site format and any previous crawls of the site.

*   [Review the crawl reports](https://support.archive-it.org/hc/en-us/articles/208002126-Reading-your-crawl-report), especially looking for hosts with large amounts of content that you did not want to capture and for large amounts of blocked or queued or out of scope content you had intended to capture.

*   Compare the crawled and live sites. Look for major differences such as missing images, embedded content, or formatting.

*   If you have run previous crawls of this site, you can [compare the results of each crawl](https://support.archive-it.org/hc/en-us/articles/208333933-Compare-two-separate-crawls-).

*   If you didn't get what you want, adjust the scope (see Step 5) and run another crawl.

    * You might also [crawl missing pages as separate seeds](https://support.archive-it.org/hc/en-us/articles/208333833-Quality-Assurance-Overview#Crawl).

    * For errors in capturing dynamic content try [a Brozzler crawl instead](https://support.archive-it.org/hc/en-us/articles/360000351986-How-and-when-to-use-Brozzler).

    * You can add notes to the crawl in Archive-It as a record of what didn't work by clicking "notes" on the [crawl overview tab](https://support.archive-it.org/hc/en-us/articles/208002126-How-to-read-your-crawl-s-report).

*   [Save the test crawl](https://support.archive-it.org/hc/en-us/articles/208001226-Run-monitor-and-save-a-test-crawl) once you are satisfied with what was captured.


## 7. Add Seed Metadata

*   Use the [UGA Web Archives Metadata Profile](metadata_profile.md) to determine what information to include in any description of web archives.

*   Describe the site even if we cannot provide access yet, but do include a rights statement with the restriction information.

*   Add metadata to Archive-It for [the seed](https://support.archive-it.org/hc/en-us/articles/360014464192-Add-and-Edit-Seed-Level-Metadata-). You can also [batch add or update seed metadata](https://support.archive-it.org/hc/en-us/articles/208012996-Upload-and-download-metadata) via a spreadsheet. This must be completed prior to the quarterly preservation downloads.

*   Add a description of the archived site in the finding aid if there is a related collection. We generally add web archives as a separate series since the wide variety of content in a site is unlikely to fit into an existing series.


## 8. Make the Seeds Public

*   [Access to content](https://support.archive-it.org/hc/en-us/articles/208334003-Controlling-access-to-your-web-archives-) on the [Archive-It public page](https://support.archive-it.org/hc/en-us/articles/208002196-Browse-and-search-on-archive-it-org) is controlled by making a collection or seed private or public.

*   Staff can still view private collections and seeds when they are logged in.

*   A private seed can be located within a public collection and will not be visible online until it is public.

*   You can change the private/public status of a[ single seed](https://support.archive-it.org/hc/en-us/articles/208334003-Controlling-access-to-your-web-archives-#Howtorestrictaccesstoyourwebarchives-Howtomakeaspecificseedwithinyourcollectionprivateorpublic) or a [batch of seeds.](https://support.archive-it.org/hc/en-us/articles/208334003-Controlling-access-to-your-web-archives-#Howtorestrictaccesstoyourwebarchives-Howtomakemultipleseedswithinyourcollectionprivateorpublic).


## 9. Preservation

Archive-It [provides good digital preservation](https://support.archive-it.org/hc/en-us/articles/208117536-Archive-It-Storage-and-Preservation-Policy) for the copies they maintain. Additionally, the UGA Libraries Archive-It Administrator downloads all WARCs and six selected metadata reports each quarter to store in our local preservation system (ARCHive) to have control over these critical resources.


<!-- Docs to Markdown version 1.0β19 -->
