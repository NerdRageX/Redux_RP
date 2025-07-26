# Current Development Status
Last Updated: July 26, 2023

## Active Development
- Currently working on: NPC Management System (redux_npcmanager)
- Current challenge: NPC visibility issues - NPCs are spawning but are invisible to players
- Approach being tried: Using story mode character models (cs_* prefix) which seem to load properly

## Recent Progress
- Successfully fixed syntax errors in redux_npcmanager/client.lua and redux_population/client.lua
- Identified that cs_colmodriscoll model loads correctly while other models have visibility issues
- Implemented basic NPC spawning system with interaction capabilities
- Created blips for NPCs on the map

## Next Steps
- Resolve NPC visibility issues completely
- Implement proper interaction dialog system
- Add behavior patterns for different NPC types
- Create a configuration system for easily adding new NPCs

## Critical Context
- The VORP framework is being used as the foundation
- We're building modular systems with exports for other resources to use
- NPC models with cs_* prefix seem to work better than other model types
- Current focus is on creating a robust NPC management system that other systems can build upon

## Code Status
- redux_npcmanager: Basic functionality working, fixing visibility issues
- redux_population: Fixed syntax errors, not currently in active development
- redux_speech: Has issues with BeginTextCommandPrint native which doesn't exist in RedM
