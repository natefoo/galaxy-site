---
 title: Loading Data
---
[Back to Support Hub](https://galaxyproject.org/support/)

Related topics
  
* [Downloading Data](/support/download-data/)
* [Load into a Data Library (Admin)](/data-libraries/)
* [Local Galaxy? Configure FTP Upload (Admin)](/admin/config/#ftp)

Tutorials

* [Galaxy Training Network (GTN)](https://training.galaxyproject.org/): [Data Manipulation](https://training.galaxyproject.org/training-material/topics/galaxy-data-manipulation/)

# Loading Data

## Video Tutorials

* Quick help: [**Manupulating NGS data with Galaxy: Getting Data In**](/tutorials/ngs/#getting-ngs-data-in)
* Full tutorial: [**Uploading data into Galaxy**](/tutorials/upload/)
* Dataset Collections, including creation during Upload: [**Processing many samples at once with collections**](https://galaxyproject.org/tutorials/collections/)

## GTN Tutorials

Most tutorials from the [Galaxy Training Network (GTN)](https://training.galaxyproject.org/) include one or more data upload steps.

* Start with this tutorial, section "Getting Data In", for a quick overview: [NGS Logistics](https://training.galaxyproject.org/training-material/topics/introduction/tutorials/galaxy-intro-ngs-data-managment/tutorial.html)
* Advanced **Upload** methods are covered in the tutorial topic group [Data Manipulation](https://training.galaxyproject.org/training-material/topics/galaxy-data-manipulation/)
* [Uploading data from the command-line](https://training.galaxyproject.org/training-material/topics/galaxy-interface/tutorials/cli-upload/) tutorial for uploading large data from the command-line, especially from remote systems accessible via SSH)
* All Tutorials: https://training.galaxyproject.org/

## Supplemental Step-by-Step

Data is loaded using the tools in the _**Get Data**_ tool group. Some access specific data provider sites that will load data back into your Galaxy history. To directly load your own local data or data from another source, use the tool _**Get Data → Upload File**_ (also accessible from the top of the left tool panel, as seen in the graphics below). Want to practice import/export functions with small sample data? Import the [Upload sample data history here](https://usegalaxy.org/u/usinggalaxy/h/upload).

* Each file loaded creates one dataset in the history.
* The maximum size limit is 50G (uncompressed).
* Most individual file compression formats are supported, but multi-file archives are not (`.tar`, `.zip`).
* If a `.tar` archive contains multiple datasets, only the first dataset inside the archive will upload.
* If your compressed data does not load correctly, try loading an uncompressed version.

### [Get Data: Upload](https://training.galaxyproject.org/training-material/faqs/gtn/get_data_upload.html)


### [Get Data: EBI-SRA](https://training.galaxyproject.org/training-material/faqs/galaxy/dataupload_EBI-SRA.html)

* [How to format fastq data for tools that require .fastqsanger format?](/support/fastqsanger/)
* [Understanding compressed fastq data (fastq.gz)](/support/compressed-fastq/)


### Upload tool location

![Upload tool location](/images/screenshots/Upload.png "Upload tool location")


### Upload tips

* **Data [quota](/main/#user-data-and-job-quotas) is at limit**, so _no new data can be loaded_. Disk usage and quotas are reported at _**User → Preferences**_ when logged in.
* **Password protected data** will require a special URL format. Ask the data source. Double check that it is _publicly accessible_.
* **No HTML content.** The loading error generated may state this. Remove HTML fields from your dataset before loading into Galaxy or omit HTML fields from the query if importing from a data source (such as Biomart).
* Compression types **.gz/.gzip, .bz/.bzip, .bz2/.bzip2, and _single-file_ .tar and .zip are (usually) supported -- but if your tar/zip data does not load -- download the data locally, unpack the archive, and upload the data directly.**
* Only the **first file in any compressed archive** will load as a **[dataset](/learn/managing-datasets)**.
* Data must be **< 50G** (uncompressed) to be successfully uploaded and added as a dataset to a history, from any source.
* **Is the problem the dataset format or the assigned datatype?** Can this be corrected by editing the datatype or converting formats? See [Learn/Managing Datasets](/learn/managing-datasets/) for help or watch the screencast above for a how-to example.
* **Problems in the first step working with your loaded data?** It may not have _uploaded_ completely. You can use the *Secure Hash / Message Digest* tool to verify that the file hash is the same on your local computer as it is on the Galaxy server. Consider using the [galaxy-upload]() utility, which has support for resuming interrupted uploads.
