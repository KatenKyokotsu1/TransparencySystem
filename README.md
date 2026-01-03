🧱 WallManager – Dynamic Wall Fade System for Unity (3D)

A Unity system that detects objects between the player and the camera and smoothly fades their materials to a transparent state to prevent visual obstruction in 3D scenes.

✨ Overview

WallManager uses Physics.RaycastAll to detect walls blocking the camera’s view of the player. When detected, wall materials are faded out using DOTween’s DOFade animation. Once the obstruction is removed, materials fade back to fully opaque. All behavior is Inspector-driven, modular, and optimized for 3D gameplay clarity.

🎮 Features
🔍 View Obstruction Detection

Casts a ray from the camera toward the player

Detects all objects matching a configurable LayerMask

🌫 Smooth Material Fading

Fades wall material alpha to a customizable transparency value

Returns to opacity when no longer blocking view

Uses DOTween DOFade with speed-based transitions

⚙ Fully Inspector Customizable
Field	Purpose
player	Target player Transform
sceneCamera	Scene camera reference
wallMask	Layers considered as walls
transparentAlpha	Target transparency when blocking
fadeDuration	Fade transition duration
fadeSpeed	Speed-based fade control
🧠 Active Wall Tracking

Stores faded walls in a List

Prevents duplicate fade calls

Auto-restores only when obstruction ends

⚡ Use Case

Avoid camera clipping/obstruction in third-person or top-down 3D games

Improve visibility in tight indoor or urban environments

Maintain immersion with seamless transitions

🔧 Requirements

Unity 2021.3+

DOTween installed and set up

Materials must support transparency (Fade or Transparent render mode)

💡 Tips

Enable material transparency mode for correct fading

Pair with camera follow systems for best results

Keep fade duration low for responsive gameplay feel

🧾 License

Open-source. Free to use, modify, and distribute in personal or commercial projects.
