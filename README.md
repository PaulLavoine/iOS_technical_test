# iOS Technical Test
iOS Developer Coding Interview - 2 Hour Assessment + 1 hour discussion

## Overview
**Duration:** 2h   
**Language:** Swift / SwiftUI  
**Platform:** iOS  

## Project Requirements
You are tasked with building an iOS application that displays a collection of images from a remote JSON API. The app should have the following functionality:

## Core Features
- **Network Request:** Download and parse JSON data from a provided URL
- **Image List Display:** Show a scrollable list of images
- **Random Image Selection:** Include a button in the top corner to randomly select and display an image
- **Detail View:** Display the randomly selected image in a separate view
- **Local Storage:** Implement caching mechanism for offline access
- **Retry Mechanism:** Handle network failures with retry functionality
- **Search Functionality:** Allow users to search through the product list

## Technical Specifications

### 1. Data Source
You will be provided with a JSON endpoint that returns an array of items. Each item contains:
```json
{
  "products": [
    {
      "team": 1,
      "title": "iPhone 9",
      "description": "An apple mobile which is nothing like apple",
      "thumbnail": "https://cdn.dummyjson.com/product-images/1/thumbnail.jpg",
      "image": "https://cdn.dummyjson.com/product-images/1/1.jpg"
    }
  ]
}
```
**FYI: There are some traps in the JSON, take a good look at it.**


**Mock API Endpoint:** `https://raw.githubusercontent.com/PaulLavoine/iOS_technical_test/main/inteview_test.json`

### 2. Main List View Requirements
- Display images in a list
- Show image thumbnails with titles (if there is no image, don't display the item)
- Implement search bar functionality to filter products by title

### 3. Random Selection Feature
- Add a button in the top-right corner (dice icon)
- When tapped, randomly select one item from the currently displayed/filtered data
- Navigate to a detail view showing the selected image

### 4. Detail View Requirements
- Display the full-size image
- Show the title and description (or nothing if there is no title)
- Include navigation back to the main list

### 5. Local Storage Requirements
- **Caching Strategy:** Implement local storage to cache downloaded data and images
- **Offline Access:** Allow users to browse previously loaded content when offline
- **Data Persistence:** Use Core Data, UserDefaults, or file system to store product information
- **Image Caching:** Cache thumbnail and full-size images locally

### 6. Retry Mechanism Requirements
- **Network Error Handling:** Implement automatic retry for failed network requests
- **User-Initiated Retry:** Provide manual retry option through UI (pull-to-refresh or retry button)
- **Error States:** Display appropriate error messages and loading states

## Bonus Points
Extra consideration will be given for:
- **Async/Await:** Modern concurrency patterns for network operations
- **Testing:** Show us how you would test this code (Unit tests)
- **Swift 6 Formatting:** Latest Swift language features and formatting standards
- **MVVM + Clean Architecture:** Clean separation of concerns
- **Advanced UI:** Proper design or/and Animations

## Technical Assessment Criteria
This assessment evaluates:
- **Networking:** JSON parsing, async operations, error handling
- **UI Implementation:** SwiftUI components, navigation, responsive design
- **Architecture:** Code organization, separation of concerns, scalability
- **Data Management:** Local storage, caching strategies, data persistence
- **Performance:** Efficient image loading, memory management, smooth scrolling
- **User Experience:** Loading states, error handling, offline functionality

## Notes
This is a comprehensive technical assessment designed to evaluate iOS development skills including modern networking patterns, robust error handling, efficient data management, and thoughtful user experience design.

✅ At the end of the 2-hour assessment, please send your completed project to:
📧 paul.lavoine@aspora.com