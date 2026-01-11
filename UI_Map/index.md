# UI Map

This document serves as a requirement list for how the player can navigate between each screen and the various elements available in each screen.
To render this diagram, use Mermaid in VS Code (Recommended).

## Navigation
```mermaid 
graph TB

    

    subgraph coreAquariumView["Core Aquarium View"]
        BuyBar
        PauseButton["Pause Btn"]
        EscMenu["Escape Menu"]
        
    end

    
    
    subgraph shopView["Shop View"]
        npcRequests["NPC Requests"]
        decorate["Decorate Btn"]
        EscMenu2["Escape Menu"]
    end
    
    subgraph decorateView["DecorateView"]
        decor["View all decor unlocked"]
        tanks["View all tanks unlocked"]
        monsters["View all monsters discovered"]
        decoratetank["decorate a tank"]
        EscMenu3["Escape Menu"]
    end

    subgraph mainMenu["Main Menu"]
        startGame["New Game Btn"]
        loadGame["Load Game Btn"] 
        options["Settings Btn"]
        VersionText
    end

    subgraph escapeMenu["Escape Menu"]
        Return("Return Btn")
        SaveGame("Save Game Btn")
        ExitGame("Exit Game Btn")
        VersionText2["Version Text"]
    end

    mainMenu --> coreAquariumView
    mainMenu --> shopView
    shopView --> decorateView




```