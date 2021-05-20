
# sbox-inspector
UI Panel Inspector for S&amp;box

[![Watch the video](https://i.imgur.com/VkO3jTu.png)](https://imgur.com/74YTzRR)

![20210519202030_1](https://user-images.githubusercontent.com/5273873/118908963-ec849480-b8e7-11eb-96e4-ba49a40b3c9b.jpg)
![20210519202053_1](https://user-images.githubusercontent.com/5273873/118908968-ed1d2b00-b8e7-11eb-9a17-1e7c3234a7de.jpg)

## Installation

Drag the `ui` folder into the `code` folder of your gamemode. Ex. `minimal/code/ui`

## Usage

Add the following to the setup of your main gamemode hud. Toggle by entering `inspector` in console.

```csharp
RootPanel.AddChild<Inspector>();
```

Example:
```csharp
public MinimalHudEntity()
{
  if ( IsClient )
  {
    RootPanel.SetTemplate( "/minimalhud.html" );
    RootPanel.AddChild<ChatBox>();
    ...
    RootPanel.AddChild<Inspector>();
  }
}
