#### Current Minecraft Server: :basecamp: __v1.21.4__  

## Directory
- [PacMan](https://github.com/Ithavollr/PacMan): Content Packs (client resource & server data)
- [GitHub Pages](https://github.com/Ithavollr/Ithavollr.github.io): Website Source Code
- [ClientModpack](https://github.com/Ithavollr/ClientModpack): As it says


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
    - [ ] Alchemy: Philosopher's stone - base health & hunger regen?
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
- Server
  + [Aincrad](https://github.com/Ifiht/Aincrad): WIP!! PaperMC fork aimed at adding new content/bug fixes.
- Tools
  + [unsup](https://git.sleeping.town/unascribed/unsup): Handles synchronization of all client environments.
  + [packwiz](https://packwiz.infra.link/tutorials/creating/adding-mods/): Organize and update client modifications. Syncs via unsup.
- Shader packs
  + [Complementary](https://modrinth.com/shader/complementary-reimagined): Best shader pack out there.
  + [Euphoria](https://modrinth.com/mod/euphoria-patches): Adds useful options to Complementary.
- Data packs
  + see [PacMan](https://github.com/Ifiht/PacMan): Merges all data packs into one monolithic pack for the server.
- Resource packs
  + see [PacMan](https://github.com/Ifiht/PacMan): Merges all resource packs into one monolithic pack for the client.
- Plugins
  + [Cardinal](https://github.com/Ifiht/Cardinal): Master plugin for Ithavollr. All other plugins are organized under its hierarchy.

