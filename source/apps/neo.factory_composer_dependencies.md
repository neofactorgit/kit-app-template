# Dependency Requirements for mockup_v7.usd in Kit 106.5

The Kit 106.5 Composer template has compatibility issues with mockup_v7.usd due to missing and deprecated dependencies. This document tracks the extensions needed to restore full functionality that was available when mockup_v7.usd was originally created.

Below is the working list of required extensions to load in Kit:


Added:
omni.kit.scriptnode - autoload
omni.kit.scripting - installed, loaded, autoload
omni.anim.graph.bundle - installed, loaded, autoload
    omni.anim.graph.core
    omni.anim.graph.schema
    omni.anim.graph.ui
omni.anim.navigation.bundle
    omni.anim.navigation.schema
    omni.anim.navigation.core # need to see if this is loaded before meshtools
    omni.anim.navigation.ui
    omni.anim.navigation.meshtools # Error: omni.anim.navigation.core is not loaded
omni.anim.skeljoint
omni.graph.visulalization.nodes
omni.anim.asset (this gets installed by something else)
omni.anim.behavior.schema (this gets installed by something else)
omni.graph.action_nodes (this won't install for some reason)
omni.anim.retarget.bundle
    omni.anim.retarget.core
    omni.anim.retarget.preview
    omni.anim.retarget.ui
omni.usd.schema.omniscripting (this gets installed by something else)


To be added:
Features:
omni.anim.motion_path.bundle
omni.kit.tool.measure


examples:
omni.kit.browser.asset
omni.simready.explorer
omni.kit.graph.editor.example
omni.graph.tutorials
omni.graph.examples.cpp


unsure:
omni.kit.graph.delegate.neo
omni.app.hydra
