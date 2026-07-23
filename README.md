# As Windows continues down the path of enslopification, has the year of the Linux desktop finally arrived?
## Preface
### A new wave of interest
It's no secret that the Windows ecosystem has been in a continuous backslide in terms of quality since the release of Windows 8 (or Vista depending on who you ask). This is a trend that started long before the move to AI, primarily driven by Microsoft's monopoly when it comes to general desktop computing. With [up to 30% of new code](https://www.cnbc.com/2025/04/29/satya-nadella-says-as-much-as-30percent-of-microsoft-code-is-written-by-ai.html) added to Windows being written by AI, this decay seems to have only accelerated, user dissatisfaction has even reach the point that it's been [acknowledged by Microsoft](https://www.windowscentral.com/microsoft/windows-11/windows-11-major-improvements-announced-movable-taskbar-less-ads-reduced-copilot-better-performance-2026).

While many tech-savvy Windows users show interest in moving over to Linux, until recently nothing has really pushed them to make the jump. \
However, with the end of support for Windows 10, there's been an [uptick in discussion](https://www.reddit.com/r/linuxquestions/comments/1j7h6vk/can_i_get_some_of_you_guys_pros_cons_from/) from people who have made that switch, or are looking to do so. While there are many people who are incredibly happy to leave Windows behind, a not insignificant amount also end up running into issues with Linux and [switch back](https://www.reddit.com/r/linux_gaming/comments/1rvdmqz/i_regrettably_switched_back_to_windows/) to Windows.

Even for those that do stick with Linux, a consistent complaint seems to be how unfriendly the [installation and new user experience](https://www.reddit.com/r/linux4noobs/comments/1g66zuh/new_user_experience_installing_and_getting_started/) is compared to Windows.

### What makes a "bad" new user experience?
Much of the unwelcoming nature of the new user experience within the Linux ecosystem has been chalked up to "that's just how Linux works". This attitude shifts the burden away from obtuseness in UX design onto the user needing to learn. While to some degree this is true and there _are_ many operational conventions that differ from Windows and will need to be relearned like the use of a package manager for software, there's a lack of signposting that makes it hard for people to even know what they don't know.

Most people want to learn new things!

Many of the issues new users have when it comes to learning and troubleshooting are a result of not knowing where to even begin or what to ask in the first place. This can especially be an issue with the majority of desktop enviroments having now moved from X11 to Wayland, a lot of the solutions people find for common issues may not even be applicable anymore. The proliferation of Flatpak can also cause a lot of confusion as well, most GUI wrappers for package managers don't make it clear when you enable Flatpaks in them that the applications are sandboxed and may require you to download something like Flatseal to allow it to interact with the rest of your operating system.

While coming up with a solution for these two examples is largely outside of the scope of this case study and will likely be resolved over time with further maturation of the platform, they work well to illustrate a more general problem across the Linux ecosystem of new users being able to encounter problems which require prerequisite knowledge of how the underlying system works to even look up their issue in the first place.

Smaller points of friction also exist due to fragmentation of the platform. Someone trying to figure out how to enable dark mode may be toggling it on for GTK applications and become frustrated it's not working because they're unaware the application they're trying to change uses QT.

### Goals

Due to the nature of open source and what is being studied, there won't be any definitive answers or solutions to larger linux ecosystem issues being proposed. This primarily serves as an analysis of the current landscape and to document of some of the possible issues and pain points that someone who is more familiar with Windows and migrates to Linux may encounter. 

Examples of possible changes to smooth over more minor points of friction encountered in usability testing will be provided, but the scope of these will be limited to smaller changes to the existing onboarding experience of the distros tested.

## Biases and limitations of this case study

### Time frame
This was planned and put together in only a week. With more time I would have liked to planned a more structured usability test and built prototypes for user feedback on possible changes. I would have also performed more preliminary research and collected more external citations and data from a wider variety of online communities.

### Lack of existing data
While searching for pre-existing data, there seemed to be a lack of publicly accessible studies and survey results on this topic. The [Fedora User and Contributor Survey](https://discussion.fedoraproject.org/t/fedora-user-and-contributor-survey-now-open/155729) results for 2025 don't seem to be released. I reached out to the contact listed on the survey regarding them, but have yet to recieve a reply. For data specifically regarding the Anaconda installer, I was able to find [usability test results](https://fedoraproject.org/w/uploads/1/1f/Brno-Session1-Rreport.pdf) from the 2013 [UX Redesign](https://fedoraproject.org/wiki/Anaconda/UX_Redesign) for Fedora 19, but I was unable to find the results of the survey from then. As the data is 13 years old and for a previous version of Anaconda, it was primarily used as a reference for formulating my own case study.

### Sample pool biases
This case study has been independently designed and conducted entirely by myself without the support of any institutions. This has limited my outreach and the user participation to my friends and their social circles. This skews sampling biases towards people who do creative work like music production, digital art, and game development.

### Survey response
Getting people to respond to [my survey](https://forms.gle/wQHy6iMmnYMQkr8m6) has been a challenge. While some insights have been gained from the responses received so far, I do not feel as if a sufficient number of responses have been gathered to establish overarching narratives or larger trends in the data. Once enough responses have been received, the survey will be closed and this document will be updated.

### Usability testing participation
At this time usability testing has only been conducted with _**1**_ user. There are plans to conduct them with _**2**_ more users and potential interest from a third, but due to scheduling conflicts I was unable to perform them before putting this out. The repo for this case study will be updated with notes from those usability tests once they're conducted. Ideally I would like to find a 5th user to be thorough in my usability testing and conform to the Nielsen Norman Group methodology.

### Scope of inquiry and open-endedness

The Linux onboarding experience covers an incredibly broad number of use cases and scenarios and the question of when can a user be considered to have "fully moved" to Linux can stretch out as they find little things to fix or perform more infrequent tasks. Usability testing is also being performed on participant's personal machines so distributions chosen and tasks being performed are individualized based on my own personal opinions of what is the best fit their workflows and personal needs.

## Lessons from usability testing

### Participant 1

#### Background 
- Has used Windows for the past 30 years start with Windows 3.1.
- Primary desktop use case is general web browsing, playing games, and game development.
- Consider themselves highly confident when it comes to their technical skills with Windows.
- Exposure to Linux is limited to them running it off a live CD for a few weeks when they needed to take notes for class and their hard drive was broken. 

Primary motivation for deciding to to move off Windows is: \
"Windows has gotten slower, windows updates have caused my computer issues numerous times. It's been bloated with unnecessary AI features such as Copilot and the search functionality has become infinitely worse since the days that I could just tap the windows key and type a file name. I've had a windows update nearly brick my work computer earlier this year."

#### Fedora with KDE Plasma
Originally I had them attempt to install Fedora, primary reasons being they didn't want to tinker too much and wanted something stable, but also with their primary uses cases more frequent release cycle would likely provide better compatibility with newer releases of Proton and Gamescope compared to something like Debian with more infrequent releases. 

Starting from the Fedora website, there wasn't any download button immediately visible on screen so they selected the "Get Fedora" in the above navbar. Their first instinct was to select the Workstation edition. Asking them why they chose that one, they stated that the text under KDE Plasma stating "The next generation personal desktop." made them think that it was the unstable version.

![Screenshot: Navbar with "Get Fedora" selected and a table of the editions of Fedora available below.](example-pictures/getfedora.png)
_The various editions of Fedora available with brief descriptions._

I directed them to return to the homepage and scroll down at which point they saw the boxes with expanded descriptions and clicked on "Learn More" for the Workstation edition. After looking through screenshots they commented that it "Looked like macOS" and clicked the back button to go look at the KDE Plasma edition. After scrolling down to look through they screenshots, they said that it looked more like Windows and clicked the Download button.

After downloading the ISO, there was some confusion on what to do with it. They first attempted to just drop the ISO on a USB drive, but due to time contraints, I informed them that they wouldn't work. They proceeded to Google "how to install an iso". After reading they began to look for utilities to write it to USB. I informed them that there was a link to a program that could do it on the Fedora download page. They then returned to the download page and clicked on the link to download Fedora Media Writer which took them to a GitHub page, there was about 30 seconds of hesitation as they tried to find the download link.

_UX improvement suggestion: The download process could likely be streamlined by directly linking to the file download instead of directing to a GitHub download page._

The process of writing the ISO to the went smoothly. After doing so they rebooted into their live enviroment. There was some initial concern from them due to having a multi-monitor setup and the screen being duplicated across both their displays. This quickly fixed itself but then there was some annoyance due to their smaller non-primary monitor being treated as the primary one.

The next point of friction occured when the user attempted to install to their Hard Drive. When attempting to install they clicked the "Next" button as they thought the Fedora icon in the center was just an image and it wasn't immediately obvious that it was a button.

_UX improvement suggestion: Place an Install button beside the Next button with updated information text stating what the Next button does._

<img src="example-pictures/installbutton.png" alt="Screenshot: Fedora Welcome Center with a large icon of the Fedora logo in the center with text below stating 'Install to Hard Drive'" width="80%"> \
_Before_

<img src="example-pictures/installbuttonedit.png" alt="Screenshot: The same image as above, however the text below the logo has been removed and there is now an install button at the bottom" width="80%"> \
_After_

<p float="left">
  <img src="example-pictures/installscreen.png" alt="" width="49%" />
  <img src="example-pictures/installreview.png" alt="" width="49%" />
  <i>Before</i>
</p>



<p float="left">
  <img src="example-pictures/installscreenedit.png" alt="" width="49%" />
  <img src="example-pictures/installreviewedit.png" alt="" width="49%" />
  <i>After</i>
</p>


<img src="example-pictures/setupscreen.png" alt="" width="80%" /> \
_Before_

<img src="example-pictures/setupscreenedit.png" alt="" width="80%" /> \
_After_

### WIP

## Final thoughts

### WIP
