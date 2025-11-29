#### Current Minecraft Server: :basecamp: __v1.21.4__  

## Project Overview
- [Aincrad Server](https://github.com/Ithavollr/Aincrad)
  - **Description**: Content Packs (client resource & server data)
- [Cardinal Plugin](https://github.com/Ithavollr/Cardinal)
  - **Description**: Server management plugin, handles world-specific things that should not go into NMS
  - **Workflows**: ![JUnit Tests](https://github.com/Ifiht/Cardinal/actions/workflows/gradle.yml/badge.svg)
- [Yui Mod](https://github.com/Ithavollr/Yui)
  - **Description**: Client mod (Fabric) needed to sync changes to NMS on the backend
  - **Workflows**: ![Build](https://github.com/Ithavollr/Yui/actions/workflows/gradle.yml/badge.svg)
- [PacMan](https://github.com/Ithavollr/PacMan)
  - **Description**: Content pack auto-generator (client resource pack & server data pack)
  - **Workflows**: ![Package](https://github.com/Ithavollr/PacMan/actions/workflows/makefile.yml/badge.svg) ![Package](https://github.com/Ithavollr/PacMan/actions/workflows/runserver.yml/badge.svg)
- [GitHub Pages](https://github.com/Ithavollr/Ithavollr.github.io): 
  - **Description**: Website Source Code
- [ClientModpack](https://github.com/Ithavollr/ClientModpack)
  - **Description**: Bundled auto-updating client modpack managed by unsup


## TO-DO:
See the [Dev Board](https://github.com/orgs/Ithavollr/projects/1/views/1)
- [ ] Add back [RP-Renames](https://modrinth.com/mod/rp-renames) for 1.21.4 when available
- [ ] Add Potion of Flying
- [ ] **Add back AuraSkills**
  - [ ] Implement client-side interface
  - [ ] Give users 3 skill points
  - [ ] Limit to 3 active skills chosen by skill point
  - [ ] Erase skill xp when switching skills
  - [ ] Implement "ultimate" skill unlocks @lvl 99
    - [ ] Agility: Charged Jump
    - [ ] Alchemy: Philosopher's stone - XP regen
    - [ ] Archery: Permanent Infinity
    - [ ] Defense: Mana/Exp Shield
    - [ ] Enchanting: ???
    - [ ] Excavation: Terraform
    - [ ] Farming: Instant Plant Growth
    - [ ] Fighting: ???
    - [ ] Fishing: Water Breathing
    - [ ] Foraging: "Friend of the Forest" - all mobs neutral while active
    - [ ] Mining: Speed Mining

## Project Workflow:
```
                                                                      
               ┌──────────┐                                           
               │ Cardinal ├───────┐                                   
               └──────────┘       │                                   
                                  │           ┌────────────────────┐  
                                  │           │  Minecraft Server  │  
                                  ├──────────►│      (Aincrad)     │  
                                  │           └────────────────────┘  
 ┌─────────────┐                  │                                   
 │   PacMan    ├───┬──────────────┘                                   
 └─────────────┘   │                                                  
                   │                         ┌──────────────────────┐ 
                   │   ┌──────────┐          │   Minecraft Client   │ 
                   ├──►│ PrismPak ├─────────►│ (via Prism Launcher) │ 
                   │   └──────────┘          └──────────────────────┘ 
                   │                                                  
 ┌─────────────┐   │                                                  
 │ClientModpack├───┘                                                  
 └─────────────┘                                                      
                                                                      
```
## References
- Tools
  + [unsup](https://git.sleeping.town/unascribed/unsup): Handles synchronization of all client environments.
  + [packwiz](https://packwiz.infra.link/tutorials/creating/adding-mods/): Organize and update client modifications. Syncs via unsup.
- Shader packs
  + [Complementary](https://modrinth.com/shader/complementary-reimagined): Best shader pack out there.
  + [Euphoria](https://modrinth.com/mod/euphoria-patches): Adds useful options to Complementary.
- Resource packs:
  + [Roundista](https://modrinth.com/resourcepack/roundista): Best resource pack for upgrading the look & feel of vanilly game textures.


