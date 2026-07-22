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
Getting people to respond to [my survey](https://forms.gle/wQHy6iMmnYMQkr8m6) has been a challenge. While some insights have been gained from the responses received so far, I do not feel as if a sufficient number of responses have been gathered to establish overarching narratives or larger trends in the data. Once enough responses have been received, the survery will be closed and this document will be updated.

### Usability testing participation
At this time usability testing has only been conducted with _**1**_ user. There are plans to conduct them with _**2**_ more users and potential interest from a third, but due to scheduling conflicts I was unable to perform them before putting this out. The repo for this case study will be updated with notes from those usability tests once they're conducted. Ideally I would like to find a 5th user to be thorough in my usability testing and conform to the Nielsen Norman Group methodology.

### Scope of inquiry and open-endedness

The Linux onboarding experience covers an incredibly broad number of use cases and scenarios and the question of when can a user be considered to have "fully moved" to Linux can stretch out as they find little things to fix or perform more infrequent tasks. Usability testing is also being performed on participant's personal machines so distributions chosen and tasks being performed are individualized based on my own personal opinions of what is the best fit their workflows and personal needs.

## Lessons from usability testing

### WIP

## Building a better onboarding experience for new users

### WIP

## Final thoughts

### WIP
