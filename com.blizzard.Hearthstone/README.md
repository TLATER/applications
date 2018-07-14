# Hearthstone
A fast-paced strategy card game

## Status

| Arch  | Installs | Runs | Notes                                                            |
| ----- | -------- | ---- | ---------------------------------------------------------------- |
| 32bit | N/A      | N/A  |                                                                  |
| 64bit | Yes      | Yes  | After installation, the battle.net client *must* first be closed |

## Build & Install
### Repo
#### 32bit

    flatpak-builder --arch=i386 --force-clean builds --repo=winepak com.blizzard.Hearthstone.yml
    flatpak --user install winepak com.blizzard.Hearthstone

#### 64bit

    flatpak-builder --arch=x86_64 --force-clean builds --repo=winepak com.blizzard.Hearthstone.yml
    flatpak --user install winepak com.blizzard.Hearthstone

### Direct
#### 32bit

    flatpak-builder --user --arch=i386 --force-clean --install builds com.blizzard.Hearthstone.yml

#### 64bit

    flatpak-builder --user --arch=x86_64 --force-clean --install builds com.blizzard.Hearthstone.yml

## Run

    flatpak run com.blizzard.Hearthstone

    Note: Make sure that during the first run, you close the battle.net launcher
          before signing in. It will be relaunched for you, after which you
          can use the client as you would normally do.
