# Pre-work - SimpleToDo

SimpleToDo is an android app that allows building a todo list and basic todo items management functionality including adding new items, editing and deleting an existing item.

Submitted by: Sreelakshmi Gownipalli

Time spent: 10 hours spent in total

## User Stories

The following **required** functionality is completed:

* [X] User can **successfully add and remove items** from the todo list
* [X] User can **tap a todo item in the list and bring up an edit screen for the todo item** and then have any changes to the text reflected in the todo list.
* [X] User can **persist todo items** and retrieve them properly on app restart

The following **optional** features are implemented:

* [ ] Persist the todo items [into SQLite](http://guides.codepath.com/android/Persisting-Data-to-the-Device#sqlite) instead of a text file
* [ ] Improve style of the todo items in the list [using a custom adapter](http://guides.codepath.com/android/Using-an-ArrayAdapter-with-ListView)
* [ ] Add support for completion due dates for todo items (and display within listview item)
* [ ] Use a [DialogFragment](http://guides.codepath.com/android/Using-DialogFragment) instead of new Activity for editing items
* [ ] Add support for selecting the priority of each todo item (and display in listview item)
* [ ] Tweak the style improving the UI / UX, play with colors, images or backgrounds

The following **additional** features are implemented:

* [ ] List anything else that you can get done to improve the app functionality!

## Video Walkthrough

Here's a walkthrough of implemented user stories:

http://i.imgur.com/YJNOxfy.gifv

GIF created with [LiceCap](http://www.cockos.com/licecap/).

## Project Analysis

As part of your pre-work submission, please reflect on the app and answer the following questions below:

**Question 1:** "What are your reactions to the Android app development platform so far? Compare and contrast Android's approach to layouts and user interfaces in past platforms you've used."

**Answer:** Android studio is easy to use compared to other platforms i have used. It is quite convinient to add user interface elements,define its properties ,running the app and debugging is easy. 

**Question 2:** "Take a moment to reflect on the `ArrayAdapter` used in your pre-work. How would you describe an adapter in this context and what is its function in Android? Why do you think the adapter is important? Explain the purpose of the `convertView` in the `getView` method of the `ArrayAdapter`."

**Answer:**  Adapter is an interface whose implementations provide data and control the display of that data. ListViews own adapters that completely control the ListView’s display. So adapters control the content displayed in the list as well as how to display it.convertview is used to increase the performance of  Adapter. When a ListView uses an Adapter to fill its rows with Views, the adapter populates each list item with a View object by calling getView() on each row. The Adapter uses the convertView as a way of recycling old View objects that are no longer being used. In this way, the ListView can send the Adapter old, "recycled" view objects that are no longer being displayed instead of instantiating an entirely new object each time the Adapter wants to display a new list item. This is the purpose of the convertView parameter.

## Notes

Describe any challenges encountered while building the app.
The big challenge i encountered is how to pass data from one activtiy window to other and how to writeback that data.Also some difficulty in understanding about onclickitemlistener.

## License

    Copyright [2017] [Sreelakshmi Gownipalli]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
