# SD Updates (3)
->Only news here<-
->Find downloads and links here: https://rentry.org/sdgoldmine<-
->Old stuff here https://rentry.org/oldsdupdates<-

All rentry links are ended with a '.org' here and can be changed to a '.co'. Also, use incognito/private browsing when opening google links, else you lose your anonymity / someone may dox you

## Contact

If you have information/files (e.g. embed) not on this list, have questions, or want to help, please contact me with details

Socials: 
Trip: questianon !!YbTGdICxQOw 
Discord: malt#6065
Reddit: u/questianon
Github: https://github.com/questianon
Twitter: https://twitter.com/questianon

!!! note Update instructions. If SD breaks go backward in commits until it starts working again
	Instructions:
	* If on Windows:
		1. navigate to the webui directory through command prompt or git bash
			a. Git bash: right click > git bash here
			b. Command prompt: click the spot in the "url" between the folder and the down arrow and type "command prompt". 
			c. If you don't know how to do this, open command prompt, type "cd [path to stable-diffusion-webui]" (you can get this by right clicking the folder in the "url" or holding shift + right clicking the stable-diffusion-webui folder)
		2. ```git pull```
		3. ```pip install -r requirements_version.txt```
	* If on Linux: 
		1. go to the webui directory
		2. ```source ./venv/bin/activate```
			a. if this doesn't work, run ```python -m venv venv``` beforehand
		3. ```git pull```
		4. ```pip install -r requirements.txt```
	
	If AUTOMATIC1111's Github goes down, you can try checking his alt repo: https://gitgud.io/AUTOMATIC1111/stable-diffusion-webui
		
>2/23
- US Copyright Office state that images produced by Midjourney for "Zarya of the Dawn" is not eligible for copyright protection as they did not meet the minimum human authorship requirements, however the story and arrangement of the images in the comic is eligible for copyright protection
	- In short, copyright of AI images (in the US at least) is still muddy.
	- Correspondence letter: https://fingfx.thomsonreuters.com/gfx/legaldocs/klpygnkyrpg/AI%20COPYRIGHT%20decision.pdf
	- Post: https://processmechanics.com/2023/02/22/a-mixed-decision-from-the-us-copyright-office/ 
	- Reddit post: https://www.reddit.com/r/StableDiffusion/comments/1196wl6/us_copyright_office_affirms_copyright_of/
	- Extra law information: https://www.reddit.com/r/bigsleep/comments/uevfch/article_ai_authorship_by_a_law_professor_2020/

>2/22
- Huggingface adds a diffusion model gallery: https://huggingface.co/spaces/huggingface-projects/diffusers-gallery
- OpenAI tries to restrict language models and open source projects: https://arxiv.org/pdf/2301.04246.
	- https://twitter.com/harmlessai/status/1624617240225288194
	- Reddit: https://www.reddit.com/r/StableDiffusion/comments/111fbvb/closedai_strikes_again
- A1111 released an auto installer for his webui: https://github.com/AUTOMATIC1111/stable-diffusion-webui/releases/tag/v1.0.0-pre
- InstructPix2Pix built into A1111's webui
	- IP2P is a model that can make changes to an image use natural language prompts
		- https://www.timothybrooks.com/instruct-pix2pix
	- Model download: https://huggingface.co/timbrooks/instruct-pix2pix/tree/main
	- Reddit post with more information: https://www.reddit.com/r/StableDiffusion/comments/10tjzmf/instructpix2pix_is_built_straight_into_the/
- ControlNet + Houdini (3D software) extension wip
	- https://www.reddit.com/r/StableDiffusion/comments/115eax6/im_working_on_api_for_the_a1111_controlnet/
- LORA training guide: https://i.imgur.com/J8xXLLy.png
	- https://www.reddit.com/r/StableDiffusion/comments/110up3f/i_made_a_lora_training_guide_its_a_colab_version/
- ControlNet guide: https://i.redd.it/a2ifnjcqj4ja1.png
- 2 weeks old but the ControlNet extension is released
	- Neural network that adds more control over Stable Diffusion models without merging or requiring much img2img
	- Probably the largest improvement to compositional prompting (fixes hands greatly!) and img2img
	- Allows for extracting compositions and poses from images
		- You can mix this with 3D pose software like Daz3D, https://magicposer.com/, and the OpenPose extension to create characters with specific poses quickly
	- Has many different preprocessors and models
		- In recent update, you can use multiple models at once (enable this in the settings)
		- Example model: Sketch - Converts a sketch into a base for an image, retaining the basic composition
	- Has an option to guess the image provided and generate something even with no prompt
	- Simple explanation of all the settings and models: https://www.reddit.com/r/StableDiffusion/comments/119o71b/a1111_controlnet_extension_explained_like_youre_5/
	- Pruned models (good for most people): https://civitai.com/models/9868/controlnet-pre-trained-difference-models
	- Original models: https://huggingface.co/lllyasviel/ControlNet
	- Original Github: https://github.com/lllyasviel/ControlNet
	- A1111 Plugin Github: https://github.com/Mikubill/sd-webui-controlnet
- OpenPose plugin released
	- Extract pose information from images
	- Works with ControlNet
	- Github: https://github.com/fkunn1326/openpose-editor
- Attend-and-Excite: Introduces Generative Semantic Nursing to intervene during the generative process to guide the model to generate all the tokens in a prompt
	- Github: https://github.com/AttendAndExcite/Attend-and-Excite
	- Paper: https://arxiv.org/abs/2301.13826
	- Website: https://attendandexcite.github.io/Attend-and-Excite/
- Free and open source photoshop plugin released a few weeks ago
	- Github: https://github.com/AbdullahAlfaraj/Auto-Photoshop-StableDiffusion-Plugin
	- Reddit showcase: https://www.reddit.com/r/StableDiffusion/comments/10n3cqo/major_update_automatic1111_photoshop_stable/
- Big update for the NKMD GUI from a few weeks ago
	- Reddit post: https://www.reddit.com/r/StableDiffusion/comments/10kbyro/nmkd_stable_diffusion_gui_190_is_out_now/
	- Github: https://github.com/n00mkrad/text2image-gui
	- Itch.io: https://nmkd.itch.io/t2i-gui/devlog/480628/sd-gui-190-now-with-instructpix2pix
- Oldish: Google announces Dreamix
	- Generates videos from a prompt and input video
- Old: RunwayML working on video to prompt to video: https://arxiv.org/abs/2302.03011
- Super old, but relevant because of video: Layered neural networks for consistency in video: https://layered-neural-atlases.github.io/

>2/2
- Netflix short animation uses image generation for its backgrounds
	- https://twitter.com/NetflixJP/status/1620357552025538561
- Text to 3D dynamic video using 4D paper released: https://make-a-video3d.github.io/
	- Can view from any camera location and angle
- Text to Live: Image and video editing using text
	- https://text2live.github.io/
- AUTOMATIC1111 releases a pixelization extension for his webui: https://github.com/AUTOMATIC1111/stable-diffusion-webui-pixelization
- Oldish update: You can preview embeds in AUTOMATIC1111's webui
- Oldish update: Waifu Diffusion 1.4 released
	- Diffusers: https://huggingface.co/hakurei/waifu-diffusion
	- Pickle: https://huggingface.co/hakurei/waifu-diffusion-v1-4
- Old update: Extension that completes depth2img support released
	- https://github.com/AnonymousCervine/depth-image-io-for-SDWebui
- Old update that I forgot to include: VoltaML, similar to SDA, increases speeds by up to 10x (from what I've heard)
	- https://github.com/VoltaML/voltaML-fast-stable-diffusion

>1/28
- Stable Diffusion Accelerated API (SDA) released by SAIL: https://github.com/chavinlo/sda-node
	- Uses TensorRT to speed up generation speeds on NVIDIA cards
		- Generate a 512x512 @ 25 steps image in half a second
	- HTTP API
	- More schedulers from diffusers
	- Weighted prompts (ex.: "a cat :1.2 AND a dog AND a penguin :2.2")
	- More step counts from accelerated schedulers
	- Extended prompts (broken at the moment)
	- You can test it on their server before you download it: https://discord.gg/RWbpNGyN

>1/23
- Class action lawsuit filed by three artists against Stability AI, Midjourney, and Deviant Art for Stable Diffusion
	- Same lawyers as those that sued Github Copilot
	- Reddit post: https://www.reddit.com/r/StableDiffusion/comments/10bj8jm/class_action_lawsuit_filed_against_stable/
	- Youtube video I found: https://www.youtube.com/watch?v=gv9cdTh8cUo
- Low-rank Adaptation for Fast Text-to-Image Diffusion Fine-tuning (Lora) released
	- Alternative to Dreambooth, 3mb files
	- Reddit: https://www.reddit.com/r/StableDiffusion/comments/1078nsf/version_010_of_lora_released_alternative_to/
	- Github: https://github.com/cloneofsimo/lora
	- Notebook: https://github.com/cloneofsimo/lora/blob/master/scripts/run_inference.ipynb
- Safetensors seems to be the norm now, and they should be safe for you to download and use.
- Large checkpoint repository with a nice ui released: https://civitai.com/
	- Has sorting options, previews, comments, etc. Seems to be an uncensored replacement for HuggingFace?
- Android APK for generating 256x256 images from NovelAI released: https://github.com/EdVince/Stable-Diffusion-NCNN
- Various updates to ChatGPT: https://openai.com/blog/chatgpt/
- Open Assistant: Basically open source ChatGPT
	- Github: https://github.com/LAION-AI/Open-Assistant
- (Somewhat old?, relevant because of ChatGPT) Largest Open Multilingual Language Model: BLOOM
	- https://huggingface.co/bigscience/bloom
	- https://bigscience.huggingface.co/blog/bloom
- Many UI and functional updates to AUTOMATIC1111's webui, make sure to git pull/update to get them
- Old newsfeed posts have been archived: https://rentry.org/oldsdupdates

>11/26 to 12/12
- Goldmine is being reorganized and curated, update will come out when it looks organized
- Update your AUTOMATIC1111 installation for a lot of fixes + features
	- Notable updates I can find:
		- Adding --gradio-inpaint-tool and color-sketch: https://github.com/AUTOMATIC1111/stable-diffusion-webui/commit/5cd5a672f7889dcc018c3873ec557d645ebe35d0
		- Safetensors merged: https://github.com/AUTOMATIC1111/stable-diffusion-webui/pull/4930
			- To enable SafeTensors for GPU, the `SAFETENSORS_FAST_GPU environment` variable needs to be set to `1`
			- Batch conversion script is in the PR
			- Convert: https://huggingface.co/spaces/safetensors/convert
		- A bunch of UI updates/fixes
		- Proper SD 2.0 support (primary commit linked): https://github.com/AUTOMATIC1111/stable-diffusion-webui/commit/ce6911158b5b2f9cf79b405a1f368f875492044d
		- Improvements for various tools (like upscalers)
- (forgot to put this ever since it was created, but it's really good) InvokeAI, an all-in-one alternative to Automatic1111's webui, is updated with a lot of stuff: https://github.com/invoke-ai/InvokeAI
	- InvokeAI needs only ~3.5GB of VRAM to generate a 512x768 image (and less for smaller images), and is compatible with Windows/Linux/Mac (M1 & M2).
	- Has features like: UI Outpainting, Embedding Management, a unified (infinite) canvas, and an image viewer
	- Very user friendly (simple UI) and super easy to install (1-clicK)
	- Reddit: https://www.reddit.com/r/StableDiffusion/comments/zabmht/invokeai_22_release_the_unified_canvas/
- Unstable Diffusion reaches $25000 kickstarter goal for further training of SD 2.0
	- https://www.kickstarter.com/projects/unstablediffusion/unstable-diffusion-unrestricted-ai-art-powered-by-the-crowd
	- Goals:
		- Community GPU Cloud: researchers and community model makers can request compute grants and train their own models and datasets on our system, provided they will release the results open source
		- Further training using more steps and images
		- Only filtered out children to prevent misuse
- Stable Diffusion v2.1 released: https://stability.ai/blog/stablediffusion2-1-release7-dec-2022
	- https://huggingface.co/stabilityai/stable-diffusion-2-1
	- Reduced the strength of filters to allow for generating better people
- LORA - Low-rank Adaptation for Fast Text-to-Image Diffusion Fine-tuning space (based on the github from below): https://huggingface.co/spaces/ysharma/Low-rank-Adaptation
	- Dreambooth at twice the speed
	- Super small model file sizes (3-4MB)
	- Supposedly better than full fine-tuning according to author of the linked space
	- Reddit: https://www.reddit.com/r/StableDiffusion/comments/ziwwzh/lora_dreambooth_web_ui_finetune_stable_diffusion/
- Dreambooth on 6 GB VRAM and under 16 GB RAM released (LORA from above): https://github.com/cloneofsimo/lora
	- Reddit: https://www.reddit.com/r/StableDiffusion/comments/zfqkh3/we_can_now_do_dreambooth_on_a_gpu_with_only_6gb/
	- How to run on Windows natively without WSL (uses similar steps to linked guide): https://www.reddit.com/r/StableDiffusion/comments/ydip3s/guide_dreambooth_training_with_shivamshriraos/
- StableTuner, a GUI based Stable Diffusion finetuner, released: https://github.com/devilismyfriend/StableTuner
	- Easy to install and use, friendly GUI, and all-in-one finetuner/trainer
	- Reddit: https://www.reddit.com/r/StableDiffusion/comments/zd3xut/stabletuner_a_nononsense_powerful_finetuner_with/
- openOutpaint released: https://github.com/zero01101/openOutpaint
	- Open source, self-hosted, offline, lightweight, easy to use outpainting for AUTOMATIC1111's webui
	- Guide: https://github.com/zero01101/openOutpaint/wiki/SBS-Guided-Example
	- Manual: https://github.com/zero01101/openOutpaint/wiki/Manual
	- Reddit (has more features listed in comments): https://www.reddit.com/r/StableDiffusion/comments/zi2nr9/openoutpaint_v0095_an_aggressively_open_source/
- OpenAI releases ChatGPT, a language model for dialogue (info in the link): https://openai.com/blog/chatgpt/
	- Demo (requires account): https://chat.openai.com/	
- Automatic1111 adds support for SD depth model
	- Reddit: https://www.reddit.com/r/StableDiffusion/comments/zi6x66/automatic1111_added_support_for_new_depth_model/
	- Instructions on how to use by reddit user: 
		1. Download https://huggingface.co/stabilityai/stable-diffusion-2-depth (model) and place it in models/Stable-diffusion
		2. Download https://raw.githubusercontent.com/Stability-AI/stablediffusion/main/configs/stable-diffusion/v2-midas-inference.yaml (config) and place it in the same folder as the checkpoint
		3. Rename the config to 512-depth-ema.yaml
		4. Start Stable-Diffusion-Webui,z select the 512-depth-ema checkpoint and use img2img as you normally would.
- depthmap2mask extension released that can create 3d depth map masks --> supposedly better img2img
	- Seems to be an alternative to conditioning image mask weight
- Dreambooth training based on Shivam's repo extension updated to support SD v2.0 (find it in the extensions tab)
- Script to convert diffusers models to ckpt and (vice versa?) released: https://github.com/lawfordp2017/diffusers/tree/main/scripts
- AUTOMATIC1111 webui now on HuggingFace: https://huggingface.co/spaces/camenduru/webui
- Pickle Scanner GUI updated: https://github.com/diStyApps/Stable-Diffusion-Pickle-Scanner-GUI
- Dream Textures (Stable Diffusion for Blender) demo: https://twitter.com/CarsonKatri/status/1600248599254007810
	- Github: https://github.com/carson-katri/dream-textures
	- Reddit: https://www.reddit.com/r/StableDiffusion/comments/zf2b9k/absolutely_crazy_addon_in_blender_to_add_textures/
- Stable Diffusion IOS app  released: https://www.reddit.com/r/StableDiffusion/comments/z5ndpw/i_made_a_stable_diffusion_for_anime_app_in_your/
	- Offline?
	- App Store: https://apps.apple.com/us/app/waifu-art-ai-local-generator/id6444585505
- Simple Dreambooth training (but costs money) service released: https://openart.ai/photobooth
- All in one Stable Diffusion server (costs money but seems cheap and easy to use) released: https://rundiffusion.com/
	- https://www.reddit.com/r/StableDiffusion/comments/zea5rd/thank_you_to_all_the_alpha_testers/
- Waifu Diffusion 1.4 is delayed to Dec 26 due to a database issue (not SD 2.0)

>11/25+11/26
- My SD Hypertextbook, a tutorial that teaches a newcomer how to install and use Stable Diffusion, is released: https://rentry.org/sdhypertextbook
- SD 2.0 has support in AUTOMATIC1111's webui: https://github.com/AUTOMATIC1111/stable-diffusion-webui/commit/ce6911158b5b2f9cf79b405a1f368f875492044d
- (Reupload with new info) Pull request to support safetensors, the unpickleable and fast format to replace pytorch: https://github.com/AUTOMATIC1111/stable-diffusion-webui/pull/4930
	- Git checkout this commit
	- Convert your models locally: read the PR's first comment 
	- Convert your models in the cloud: https://colab.research.google.com/drive/1YYzfYZEJTb3dAo9BX6w6eZINIuRsNv6l#scrollTo=ywbCl6ufwzmW
