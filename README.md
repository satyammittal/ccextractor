![logo](https://avatars3.githubusercontent.com/u/7253637?v=3&s=100)
 
# CCExtractor


CCExtractor is a tool that produces subtitles from TV use. Global accessibility (all users, all content, all countries) is the goal. With so many different formats, this is a constantly moving target, but we intend to keep up with all sources and formats.

Carlos' version (mainstream) is the most stable branch.

## Google Summer of Code 2017
CCExtractor has applied for Summer of Code. The list of accepted organizations has not yet been published by Google but we are hopeful to be invited again to participate in this amazing program. 

If you are a student currently enrolled in university most likely you are eligible to participate. Read more at:  
- [Google Summer of Code official website ](https://summerofcode.withgoogle.com/)
- [CCExtractor's main GSoC page] (https://www.ccextractor.org?id=public:gsoc:ideas_page_for_summer_of_code_2017)


## Installation and Usage

Downloads for precompiled binaries and source code can be found [on our website](http://www.ccextractor.org?id=public:general:downloads).

Extracting subtitles is relatively simple. Just run the following command:

```ccextractor <input>```

This will extract the subtitles. 

More usage information can be found on our website:

- [Using the command line tool](http://www.ccextractor.org/doku.php?id=public:general:command_line_usage)
- [Using the Windows GUI](http://www.ccextractor.org/doku.php?id=public:general:win_gui_usage) 


## Compiling

### Debian/Ubuntu
    # make sure you have CCExtractor repository forked
    # clone repository
    sudo apt-get install -y git
    git clone https://github.com/%USERNAME%/ccextractor.git # paste your github username
    
    # installing dependencies
    sudo apt-get install -y gcc
    sudo apt-get install -y libcurl4-gnutls-dev
    sudo apt-get install -y tesseract-ocr
    sudo apt-get install -y tesseract-ocr-dev
    sudo apt-get install -y libleptonica-dev
    
    # compiling
    cd ccextractor/linux
    ./build
    
    # test your build
    ./ccextractor

### Fedora
    # make sure you have CCExtractor repository forked
    # clone repository
    sudo yum install -y git
    git clone https://github.com/%USERNAME%/ccextractor.git # paste your github username
    
    # installing dependencies
    sudo yum install -y gcc
    sudo yum install -y tesseract-devel # leptonica will be installed automatically
    
    # compiling
    cd ccextractor/linux
    ./build
    
    # test your build
    ./ccextractor

### Windows

Open the windows/ccextractor.sln file with Visual Studio (2015 at least), and build it. Configurations "(Debug|Release)-Full" includes dependent libraries which are used for OCR.

## Support

By far the best way to get support is by opening a support ticket at our [issue tracker](https://github.com/CCExtractor/ccextractor/issues). 

When creating a ticket:

- Make sure you are using the latest CCExtractor version.
- If it's a new issue (for example a video file that a previous CCExtractor version processed fine but now causes a crash), mention the last version you know was working.
- If the issue is about a specific file, make that file available for us. Don't just send us the output from CCExtractor, as we can't do anything about a screenshot that shows a crash. We need the input that actually causes it. You can upload the file to Dropbox, Google Drive, etc, and make it public so you get a download link to add to your ticket.
- If you cannot make the file public for any (reasonable) reason you can send us a private invitation (both Dropbox and Google Drive allow that). In this case we will download the file and upload it to the private developer repository.
- Do not upload your file to any location that will require us to sign up or endure a wait list, slow downloads, etc.
- If your upload expires make sure you keep it active somehow (replace links if needed). Keep in mind that while we go over all tickets some may take a few days, and it's important we have the file available when we actually need it.
- Make sure you set an alert in GitHub so you get notifications about your ticket. We may need to ask questions and we do everything inside GitHub's system.
- Please use English. 
- It goes without saying, we like polite people.

You can also [contact us by email or chat with the team in Slack](http://www.ccextractor.org/doku.php?id=public:general:support). 
    
## Contributing

You can contribute to the project by forking it, modifying the code, and making a pull request to the repository. 

## News & Other Information

News about releases and modifications to the code can be found in the `CHANGES.TXT` file. 

For more information visit the CCExtractor website: [http://www.ccextractor.org](http://www.ccextractor.org)
Edit access
