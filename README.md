# GbVideoPlayer

  

component for live audio commentaries

  

  

<img src="screen1.png" width="40%" />  <img src="screen2.png" width="40%" />

  

  

[![Version](https://img.shields.io/cocoapods/v/GbVideoPlayer.svg?style=flat)](https://cocoapods.org/pods/GbVideoPlayer)

[![Platform](https://img.shields.io/cocoapods/p/GbVideoPlayer.svg?style=flat)](https://cocoapods.org/pods/GbVideoPlayer)

  

## Installation

  

```ruby

pod 'GbVideoPlayer'

```

  

  

1. Add `GbVideoPlayer` to your `podfile` and run pod install

2. Add a `GbVideoPlayerView` to your `UIViewController` either programmatically or using storyboards.

  

## Configure STORYBOARD

  

- 'app:gbTitleOff' : Change the title when the player is active.

- 'app:gbTitleOn': Change the title when the player is idle.

- 'app:gbTextColor': Change text color.

- 'app:gbBackgroundColor': Change background color.

  

## Configure in code

  

```swift
import UIKit
import GbVideoPlayer

class ViewController: UIViewController {

    @IBOutlet weak var player: GbVideoPlayerView!

    override func viewDidLoad() {
        super.viewDidLoad()
        player.url = "https://livesportradio.com/global/livescore/playlist.m3u8"
        player.gbTitleOn = "Play audio commentary"
        player.gbTitleOff = "Stop audio commentary"
        player.gbTextColor = .white
        player.gbBackgroundColor = UIColor(red: 229/255, green: 70/255, blue: 68/255, alpha: 1)
    }
}
```

## License


GbVideoPlayer is available under the MIT license. See the LICENSE file for more info.
