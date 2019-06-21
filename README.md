# Go IOS Challenge

Altougth our VoD service is exceptional, we want to give our users the chance of play short videos offline, while they are on the tube or whatever.

To do so, our UX team has designed a quite simple interface that allow users to archive our goal.

![Example image](./example.png?raw=true)

Your main duty is to develop our new app based on the UX guidelines, taking into account the following requisites:

**Using Swift or Objective-C**

- Implement the main screen where an user can play videos.
- All videos must work offline so you need to cache them.

  - To cache videos you can assume that you'll receive a _push notification_ containing the whole playlist of videos.

  ```javascript
  {
    playlist: {
      "f61c3d7f92b199ed7f5812781ccba06f": {
        title: 'Superb sunset - Miami Beach 2017',
        url: 'https://static.xtrea.mr/media/sample1.mp4'
      },
      "05747156e369eff34cbecb40a2adda6a": {
        title: 'Unicorns and horses spining around',
        url: 'https://static.xtrea.mr/media/sample2.mp4'
      },
      "9f49077a912f958530060272d6d60d30": {
        title: 'Sam Smith, Normani - Dancing With A Stranger',
        subtitle: 'Official video (Ft. Normani)',
        url: 'https://static.xtrea.mr/media/sample3.mp4'
      },
      "f3058e6662927f1fcd17840469cfd5f3": {
        title: 'Tulips',
        url: 'https://static.xtrea.mr/media/sample4.mp4'
      },
      "27da99954cbcf488fb02a145079f3bb9": {
        title: 'Big Buck Bunny Movie',
        subtitle: 'Animated movie yeah',
        url: 'https://static.xtrea.mr/media/sample5.mp4'
      }
    }
  }
  ```

  **NOTE** Suppose that the order does not matter and the key of each video is a hash of the video file.

- You must notify the user when all videos has been cached so the user can open the app and play all videos without seen any loader or having to wait for the video to load.
- The user can discard a video by triggering a gesture on the app.
  - Only one gesture must be controlled by your code. A **swipe left** should stop the current video and play the next on the queue.

**Take into account the following aspects:**

- Have notes attached, explaining the solution.
- Deliver production ready code with instructions to compile and test the application.
- Provide a solution that could be easy to grow and easy to add new functionality.
- You can add any UX / UI improvements you consider, but we are going to focus on the requested features.
- When in doubt, act as a product owner
- [BONUS]: our UX team hadn't time either to work on the playlist view. You can see more details in the /bonus folder. It would be a plus if you could implement it.
