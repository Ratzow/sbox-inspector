# sbox-inspector
UI Panel Inspector for S&amp;box

## Installation

Drag the `ui` folder into the `code` folder of your gamemode. Ex. `minimal/code/ui`

## Usage

Add the following to the setup of your main gamemode hud.

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
