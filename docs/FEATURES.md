# Shift3D-AMD — feature overview

**Glasses-free 3D for any window on the Owl3D Shift, on GPUs where Owl3D's own 2D→3D doesn't run (AMD and others).** One exe, unofficial, no Owl3D files inside. Owl3D's Stereo 3D Playback does the eye tracking and weaving; Shift3D makes the side-by-side picture.

**Features**
- **2D → 3D for any window** — captures the window and builds side-by-side 3D with a small depth model (Depth Anything V3 Small on DirectML, works on any GPU vendor).
- **Already-SBS passthrough** — SBS video, TriDef, or games that render SBS themselves go straight through without AI. Browsers and video players switch to 3D only when fullscreen (YouTube fullscreen / F11), so the page stays usable until then.
- **Mouse and keyboard keep working on the 3D picture** — including windowed games shown enlarged: the real cursor stays inside the game window and moves in proportion, with an arrow drawn on the 3D frame, so clicks land exactly where you see them. Windowed mode is recommended on slower PCs.
- **Owl3D weave resolution** — pick 1440p or 1080p; Shift3D sets Owl3D's hidden setting automatically and turns its auto quality drop off. 1080p is noticeably lighter.
- **Depth profile** — "Smooth" (runs on the GPU that isn't driving the screen, no stutter) or "Detail" (strongest GPU); chosen automatically for your PC.
- **Window handling** — near-fullscreen windows drawn 1:1, smaller ones scaled up keeping their aspect ratio; a minimized game window is restored automatically.
- **Brightness / gamma for the 3D output only**, remembered between runs.
- **Monitor power** — the Shift has no power button: a "Monitor off" button (picker / tray / `--monitor off`) turns it off over DDC/CI, and any mouse or keyboard input turns it back on.
- Korean / English UI, tray icon, no console window.

**Hotkeys (Ctrl + Alt + …)**

| Key | Action |
|---|---|
| ↑ / ↓ | Parallax (3D strength) up / down |
| ← / → | Depth — scene further back / closer |
| Home / End | Brightness up / down (3D output only, remembered) |
| PageUp / PageDown | Gamma up / down (3D output only, remembered) |

**Requirements** — Windows 10/11 x64, DirectX 12 GPU, Owl3D Shift + Owl3D app 2.3.2 or later (Stereo 3D Playback → Side-by-side → Start). Chrome/Edge need `--disable-features=CalculateNativeWinOcclusion` so they keep drawing while covered.

Download: https://github.com/nautymac/Shift3D-AMD/releases

---

# Shift3D-AMD — 기능 설명

**Owl3D의 2D→3D가 안 되는 그래픽카드(AMD 등)에서도 Owl3D Shift로 아무 창이나 무안경 3D로 보는 프로그램.** 실행 파일 하나, 비공식, Owl3D 파일 미포함. 눈 추적과 엮기는 Owl3D의 Stereo 3D Playback이, 좌우 영상은 Shift3D가 만든다.

**기능**
- **아무 창이나 2D → 3D** — 창을 캡처해 깊이 모델(Depth Anything V3 Small, DirectML — 어떤 GPU든)로 좌우(SBS) 영상을 만든다.
- **이미 SBS인 화면은 그대로** — SBS 영상·TriDef·SBS를 직접 내는 게임은 AI 없이 통과. 브라우저·영상 플레이어는 전체 화면일 때만 3D로 바뀌어 그 전까지 페이지를 평소처럼 쓸 수 있다.
- **3D 화면 위에서 마우스·키보드 그대로** — 창 모드 게임을 확대해 보일 때도 실제 커서를 게임 창 안에 두고 비율로 움직이며 화살표를 3D 화면에 그려서 클릭이 정확히 맞는다. 낮은 사양은 창 모드 권장.
- **Owl3D 엮기 해상도** — 1440p / 1080p 선택. Owl3D의 숨은 설정을 자동으로 맞추고 자동 화질 낮춤을 끈다. 1080p가 눈에 띄게 가볍다.
- **깊이 계산 프로필** — 부드럽게(화면을 맡지 않은 GPU, 끊김 없음) / 정밀하게(가장 강한 GPU); PC에 맞춰 자동 선택.
- **창 처리** — 화면을 거의 채우는 창은 1:1, 작은 창은 비율을 지켜 확대; 최소화된 게임 창은 자동으로 되살린다.
- **밝기·감마는 3D 출력에만** 적용되고 기억된다.
- **모니터 전원** — Shift에는 전원 버튼이 없다. [모니터 끄기] 버튼(선택 화면·트레이·`--monitor off`)으로 끄고, 마우스나 키보드를 움직이면 다시 켜진다 (DDC/CI).
- 한/영 UI, 트레이 아이콘, 콘솔 창 없음.

**단축키 (Ctrl + Alt + …)**

| 키 | 하는 일 |
|---|---|
| ↑ / ↓ | 시차(입체 강도) 강하게 / 약하게 |
| ← / → | 깊이 — 화면 뒤로 / 앞으로 |
| Home / End | 밝기 올리기 / 내리기 (3D 출력만, 기억) |
| PageUp / PageDown | 감마 올리기 / 내리기 (3D 출력만, 기억) |

**필요한 것** — Windows 10/11 64비트, DirectX 12 그래픽카드, Owl3D Shift + Owl3D 앱 2.3.2 이상 (Stereo 3D Playback → Side-by-side → Start). 크롬·엣지는 `--disable-features=CalculateNativeWinOcclusion` 옵션 필요.

다운로드: https://github.com/nautymac/Shift3D-AMD/releases
