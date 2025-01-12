<div id="header" align="center">
  <img src="https://media.giphy.com/media/HUXjs8EtVdzYEH1gUn/giphy.gif" width="100"/>
</div>

<h1 align="center">PalliLink</h1>

Many studies have been done confirming the benefits of early palliative care such as improved symptom control and improved quality of care for patients. However, the World Health Organization (WHO) estimates that only about 14% of people who need palliative care receive it. One of the few major shortcomings in access to palliative care is the lack of resources and awareness of palliative care. When a patient meets with their primary care doctor or other specialist doctors, the patients receive treatment for their underlying ailments, but their symptoms, in the meantime, may be overlooked. The aim of a palliative care coordination app is to offload the responsibility of connecting patients with palliative care specialists from the primary care doctor.

We are creating PalliLink in order to make palliative care specialists more accessible for patients. Patients will be able to set up meetings with palliative care experts and easily share prescribed treatments and results with their existing primary care provider. The app will serve as a hub for all palliative care treatment results and will be the patient’s primary gateway to communicate with their palliative care provider.

PalliLink will not only provide access to palliative care specialists, but also provide an easy way for primary healthcare providers to see how patients react to care and plan repeat appointments and/or referrals to specialists
# Installation Guide
## Pre-Requisites
* Requires a computer that can run an emulator (300 MB of disk space)
* Emulator will require at least 4GB of RAM to run on its own 
* [Android Studio](https://developer.android.com/studio)
* [VS Code](https://code.visualstudio.com/) 

## Dependent Libraries that must be installed:
* Install Flutter and its dependencies following instructions from [here](https://docs.flutter.dev/get-started/install)

## Download Instructions
* Download PalliLink from [here](https://github.com/PalliLink/JID-2358-PalliLink) as either a Zip file or using Git to clone into a folder
    * See how to install git [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git). And how to clone into a folder[here](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository).
* Download and install Flutter and its dependencies. The link can be found [here](https://docs.flutter.dev/get-started/install)
* Open VS Code and download the Dart and Flutter extensions from the extensions tab.
* Upon finishing the download, restart VS Code to make sure extensions are enabled.
* Open a new terminal in VS Code and run 'pub get' to retrieve the dependencies for Flutter.

## Run Instructions
* Open VS Code and open the folder named JID-2358-PALLILINK
* Click the bottom right corner labeled as either denoting your operating system. This will open a new menu which will let you create an Android emulator. If you are unable to create an emulator, then your Android Studio may not be set up correctly.
* Once your Android emulator has been set up, you can again open that menu and click on the android device to begin the emulator.
* Wait for the emulator to begin running and then you can move to main.dart in the lib folder. 
* Click run at the top of VS Code and then either run with or without debugging. This will open a drop down where you must click on the emulator running you are running.
* Once VS Code finishes running, the PalliLink application should be running on your emulator


## Troubleshooting
* There are sometimes issues when running the emulator directly from VS Code. The emulator could begin but not fully connect to VS Code. To fix this, make sure that no emulator is running through android studio or is open. Then click on devices and cold start the emulator. This should resolve the issue but if it continues, a restart of your computer may help.
* A way to avoid the previous issue would be to open android studio dependently and starting an emulator through from there. This will take more time to start the application than directly running from VS Code. 

# Release Notes: 
## Version 1.0.0
### :health_worker: New Features:
* Implemented Chat feature
* Set up system so physicians can create chat rooms with patients
* Set up more questions for pain diary entry to assess new pain
* Created seperate graph to showcase new pains experienced by the patient

### :hammer_and_wrench: Bug Fixes:
* ParentDataWidget issue in patient details has been resolved

### :radioactive: Known Issues:
* Calendar UI has a two weeks button that will crash the app 
* The calendar when in scheduling appointments has an overflow when using a specific appointment type


## Version 0.4.0 
### :health_worker: New Features:
* Setup barebone chat UI
* Set up UI for a patient to add themselves to a specialist's patient list
* Access to a patient's pain charts is available through the detailed patient view

### :hammer_and_wrench: Bug Fixes:
* Pressing view entries for the pain diary now no longer breaks when there are 1 or no entries
* Altered previously hardcoded methods to be more flexible
* Fixed pain diary entry rebuilding bug
* Fixed physician profile navigation, preventing seeing physician home page twice when leaving profile page

### :radioactive: Known Issues:
* Calendar UI has a two weeks button that will crash the app
* The calendar when in scheduling appointments has an overflow when using a specific appointment type
* ParentDataWidget breaks when going into patient details

## Version 0.3.0 
### :health_worker: New Features:
* Week view with availability
* Patient charts visible, and connected to database
* Detailed medications/treatment view with precautions/instructions respectively
* Ability to edit practitioner profile information from physicians view
* Added reschedule and cancel appointment button
* Connected appointments to database
* Appointment details can be viewed
* Polished UI for detailed patient information
* Updated pain diary questions
* When scheduling an appointment, physicians can see a calendar view of other appointments

### :hammer_and_wrench: Bug Fixes:
* When creating a new user account, the app will no longer return an error saying account is not created if additional contact info is not filled out

### :radioactive: Known Issues:
* Calendar UI has a two weeks button that will crash the app
* The calendar when in scheduling appointments has an overflow when using a specific appointment type
* Flex widget breaks when going into patient details
* Clicking on physician profile will cause the physican home to have two instances, one before the changes were made and one after the changes are made.
* Patient chart does not work with one entry
* Patient chart introducing constant rebuilding even when not on page
 
## Version 0.2.0 
### :health_worker: New Features:
* User email authentication
* Pain diary history view
* Medications/Treatments view
* End of life planning page
* Connected detailed patient view to database
* Added additional fields to appointment scheduling view
* Allows for editing of patient information from physician's view
* Patient/Physician home redesign
### :hammer_and_wrench: Bug Fixes:
* Fixed all known pixel overflow
* Added null handling and loading screens
### :radioactive: Known Issues:
* When creating a new user account, the app will erroneously return an error saying account is not created if additional contact info is not filled out
* Calendar UI has a two weeks button that will crash the app

## Version 0.1.0 
### :health_worker: New Features: 
* Physican patient list 
* Detailed patient information view and navigation 
* Created appointment information views 
* Pain diary navigation and question setup 
* Calendar navigation and UI 
### :hammer_and_wrench: Bug Fixes: 
* Fixed pixel overflow on appointment button 
### :radioactive: Known Issues: 
* Pixel overflow on patient prescription detailed view 
* Errors while loading patient list view due to lack of null handling 
* Calendar UI has a two weeks button that will crash the app
* Create appointment doesn't have all the data



