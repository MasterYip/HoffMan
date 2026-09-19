<p align="center">
  <a href="https://masteryip.github.io/hoffman.github.io/">
    <img src="docs/assets/hoffman-readme-banner.svg" width="100%" alt="HoffMan — Hierarchical Action-Level Diffusion for Humanoid Motion Generation Control">
  </a>
</p>

<p align="center">
  <strong>Hierarchical Action-Level Diffusion for Humanoid Motion Generation Control</strong>
</p>

<p align="center">
  <a href="https://masteryip.github.io/hoffman.github.io/"><img alt="Project website" src="https://img.shields.io/badge/Project_Website-E7A12B?style=for-the-badge&logo=googlechrome&logoColor=171817"></a>
  <a href="#demos"><img alt="Demo videos" src="https://img.shields.io/badge/Demo_Videos-7895A6?style=for-the-badge&logo=youtube&logoColor=white"></a>
  <img alt="Code release coming soon" src="https://img.shields.io/badge/Code-Coming_Soon-5A5A57?style=for-the-badge">
  <a href="LICENSE"><img alt="MIT license" src="https://img.shields.io/badge/License-MIT-ECECEA?style=for-the-badge&labelColor=2F2F2D&color=ECECEA"></a>
</p>

<p align="center">
  <img alt="Harbin Institute of Technology" src="https://img.shields.io/badge/Harbin_Institute_of_Technology-5A5A57?style=flat-square&labelColor=5A5A57">
  <img alt="Shanghai Innovation Institute" src="https://img.shields.io/badge/Shanghai_Innovation_Institute-5A5A57?style=flat-square&labelColor=5A5A57">
  <img alt="RoboParty Lab" src="https://img.shields.io/badge/RoboParty_Lab-5A5A57?style=flat-square&labelColor=5A5A57">
  <img alt="Tsinghua University" src="https://img.shields.io/badge/Tsinghua_University-5A5A57?style=flat-square&labelColor=5A5A57">
  <img alt="Shanghai Jiao Tong University" src="https://img.shields.io/badge/Shanghai_Jiao_Tong_University-5A5A57?style=flat-square&labelColor=5A5A57">
  <img alt="HexLab" src="https://img.shields.io/badge/HexLab-5A5A57?style=flat-square&labelColor=5A5A57">
  <img alt="SFTR" src="https://img.shields.io/badge/SFTR-5A5A57?style=flat-square&labelColor=5A5A57">
</p>

> [!IMPORTANT]
> This repository currently provides the project overview and public demo links. Source code, trained checkpoints, and setup instructions are not available yet and will be added in a future release.

## Overview

**HoffMan** is a hierarchical action-level diffusion framework for humanoid motion generation and control. Its predictive rolling-denoising planning process jointly models future robot states and actions from proprioceptive history and optional task context. Predicted states remain inside the planning process, while the selected action is sent directly to the robot.

The project studies a single control interface for text-conditioned motion, semantic interpolation, joystick steering, and reaction to physical interaction across simulation and hardware demonstrations.

## Project preview

<p align="center">
  <a href="https://masteryip.github.io/hoffman.github.io/">
    <img src="https://masteryip.github.io/hoffman.github.io/static/images/hoffman-banner-poster.jpg" width="100%" alt="HoffMan humanoid control project preview">
  </a>
</p>

<p align="center"><sub>Open the <a href="https://masteryip.github.io/hoffman.github.io/">project website</a> for the full method overview, figures, and interactive demo collection.</sub></p>

### At a glance

- **Predictive control:** jointly predicts future state and action trajectories.
- **Rolling denoising:** reuses the planning horizon across control ticks for online generation.
- **Direct action output:** executes a selected action without a separate motion-tracking handoff.
- **Flexible conditioning:** supports task context and optional state-space guidance.
- **Simulation and hardware:** demonstrates commands, transitions, steering, and physical interaction.

## Demos

Click any preview to open the corresponding MP4 video. Videos are hosted by the public project website and are not duplicated in this repository.

<p align="center">
  <a href="https://masteryip.github.io/hoffman.github.io/static/videos/hoffman-mujoco-comprehensive.mp4">
    <img src="https://masteryip.github.io/hoffman.github.io/static/videos/posters/hoffman-mujoco-comprehensive.jpg" width="100%" alt="Comprehensive HoffMan simulation demo">
  </a>
</p>

<p align="center"><strong>Comprehensive simulation</strong><br><sub>Text commands, joystick steering, external interference, and semantic interpolation in one sequence.</sub></p>

<table>
  <tr>
    <td width="50%" align="center">
      <a href="https://masteryip.github.io/hoffman.github.io/static/videos/hoffman-behavioral-reaction.mp4"><img src="https://masteryip.github.io/hoffman.github.io/static/videos/posters/hoffman-behavioral-reaction.jpg" width="100%" alt="HoffMan hardware reaction demo"></a><br>
      <strong>Hardware · Physical interaction</strong><br>
      <sub>Walk and stand commands under external interference.</sub>
    </td>
    <td width="50%" align="center">
      <a href="https://masteryip.github.io/hoffman.github.io/static/videos/hoffman-text-walk-squat-walk.mp4"><img src="https://masteryip.github.io/hoffman.github.io/static/videos/posters/hoffman-text-walk-squat-walk.jpg" width="100%" alt="HoffMan walk squat walk hardware demo"></a><br>
      <strong>Hardware · Text control</strong><br>
      <sub>Walk, squat down, and return to walking.</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" align="center">
      <a href="https://masteryip.github.io/hoffman.github.io/static/videos/hoffman-text-walk-jog-squat.mp4"><img src="https://masteryip.github.io/hoffman.github.io/static/videos/posters/hoffman-text-walk-jog-squat.jpg" width="100%" alt="HoffMan walk jog squat hardware demo"></a><br>
      <strong>Hardware · Behavior transitions</strong><br>
      <sub>Walk, accelerate to a jog, and transition into a squat.</sub>
    </td>
    <td width="50%" align="center">
      <a href="https://masteryip.github.io/hoffman.github.io/static/videos/hoffman-joystick-steering.mp4"><img src="https://masteryip.github.io/hoffman.github.io/static/videos/posters/hoffman-joystick-steering.jpg" width="100%" alt="HoffMan joystick steering simulation demo"></a><br>
      <strong>Simulation · Joystick steering</strong><br>
      <sub>Directional steering with text-selected locomotion modes.</sub>
    </td>
  </tr>
</table>

## Resources

| Resource | Description |
|---|---|
| [Project website](https://masteryip.github.io/hoffman.github.io/) | Method overview, figures, authorship, and the complete demo gallery |
| [Public repository](https://github.com/MasterYip/HoffMan) | Official release channel for future code and model updates |
| [Demo collection](https://masteryip.github.io/hoffman.github.io/#evidence) | Simulation and hardware evidence in the browser |
| Paper and citation | Coming soon |

## Release status

The public release is being prepared. This README will be expanded with installation, model, data, and evaluation instructions when the implementation is ready. Please use the project website and this repository as the canonical public resources in the meantime.

## License

The contents of this repository are released under the [MIT License](LICENSE), unless noted otherwise.
