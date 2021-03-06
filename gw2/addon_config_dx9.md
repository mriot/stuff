# Addon config for Guild Wars 2 (dx9)

## arcdps (dps-meter)

- Download: <http://www.deltaconnected.com/arcdps/>
- Location: `/bin64/d3d9.dll`
- Verify install: `ALT+SHIFT+T` should open the options window

## gw2radial (mount-menu)

- Download: <https://github.com/Friendly0Fire/GW2Radial>
- Location: `/bin64/d3d9_chainload.dll`
- Verify install: `ALT+SHIFT+M` should open the menu

## d912pxy (dx12 proxy)

- Download: <https://github.com/megai2/d912pxy>
  - Place d912pxy folder in root and run installer -> make sure to select the right file name: d912pxy.dll
- Location: `/bin64/d912pxy.dll`
- Verify install: Overlay on first install and if "extras" is enabled in config-file `CTRL+ALT+N` should open the menu

## reshade (enhanced postprocessing)

- Download: <https://reshade.me/>
- Reminder: Backup preset
- **Note**: Use dx12 mode when using d912pxy
- Select `sweetFX` shaders
- Will be installed as `d3d9.dll` in game root folder -> Rename to `dxgi.dll`
- Modify reshade.ini to set paths to preset, shaders
- Select "performance mode" in ingame menu
- My preset: [mriots_clean_preset.ini](mriots_clean_preset.ini)

<details>
  <summary>Ingame graphic settings</summary>

  - **Animation**: High
  - **Antialiasing**: FXAA
  - **Environment**: High
  - **LOD Distance**: Ultra
  - **Reflections**: None (massive performance boost)
  - **Textures**: High
  - **Render Sampling**: Native
  - **Shadows**: High
  - **Shaders**: High
  - **Postprocessing**: High
  - **Char model limit**: Medium (massive performance boost)
  - **Char model quality**: Medium (massive performance boost)
  - [x] Ambient Occlusion
  - [x] Best Texture Filtering
  - [ ] Depth Blur
  - [x] Effect LOD
  - [x] High-Res Char Textures
  - [ ] Light Adaption
  - [ ] Vertical Sync (I am using G-Sync)
  - Motion blur power: Min.
</details>

---

## Alternative configs

### arcdps, d912pxy, ReShade, gw2radial

- arcdps => /bin64/d3d9.dll
- gw2radial =>/bin64/d3d9_chainload.dll
- d912pxy =>/bin64/d912pxy.dll
- ReShade => allfile => Game directory ReShade64.dll => dxgi.dll or d3d12.dll

### d912pxy, ReShade, gw2radial

- gw2radial =>/bin64/d3d9.dll
- d912pxy =>/bin64/d912pxy.dll
- ReShade => allfile => Game directory ReShade64.dll => dxgi.dll or d3d12.dll

## More

Install guides:

- <https://github.com/megai2/d912pxy/wiki/Using-with-other-addons-and-overlays>
- <https://github.com/megai2/d912pxy/issues/38#issuecomment-520420672>

Proxy config:

- <https://github.com/megai2/d912pxy/wiki/Custom-configuration>
