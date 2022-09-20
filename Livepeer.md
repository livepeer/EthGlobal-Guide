<Section name="1. Introduction" description="Introduction to Livepeer Ecosystem">

# What is the Livepeer Network

Livepeer is a decentralized video transcoding network that aims to enable cost effective, resilient, and censorship resistant video streaming.

Through storytelling, illustration, and data, the [Livepeer Primer](https://livepeer.org/primer) explains, at a high level, the problem Livepeer solves, and how it works.

# What is Livepeer Studio

[Livepeer Studio](https://livepeer.studio/) is the hosted gateway to the Livepeer Network and enables developers to quickly and easily integrate video capabilities such as live streaming, On Demand video, and video NFT minting into their applications. Developers can use [livepeer.js](https://livepeerjs.org/) or the [API](https://docs.livepeer.studio/) to build with Livepeer Studio. 

<Quiz id={"wgzm1"} />

</Section>

<Section name="2. Building with On Demand" description="How to get started with On Demand">

# Uploading an Asset
   
   Livepeer Studio's On Demand functionality allows developers to upload and playback existing video assets. This allows your users to ensure that any videos played on your frontend are opitimized for playback by reducing start up time and adapting to your users bandwidth enviornment. Additionally, video assets can be optionally stored at IPFS, so you can easily mint NFTs. 


When uploading an asset using the API, there are two methods.

- Upload with URL (providing a downloadable URL)

- Upload with local storage (provide a `.mp4` file)

When using either the SDK or dashboard for uploading an asset, only providing a `.mp4` file with H.264 video codec and AAC audio codec is required.

<Quiz id={"nn9zw"} />

---

# Updating an Asset

You can update the following attributes of an asset

1. asset name
2. storage (including IPFS)
3. metadata for the video/audio asset
   - title
   - description
   - anything you want to customize to optimize capability with your marketplace of choice


<Quiz id={"g82zv"} />


</Section>

<Section name="3. Livestream" description="Introduction to Livestreaming ">

# Building livestreaming into your application
   
Livepeer Studio makes it easy to implement live streaming video into your application. Using our Dashboard, you can test out streaming with Livepeer for yourself. 

1. [Download OBS](https://obsproject.com/), a common video encoder
1. Create an account at livepeer.studio
2. Navigate to the 'Streams' tab on the left-hand navigation
3. Click 'Create Stream' at the top right hand corner
4. Copy the RTMP ingest URL
5. Under 'Settings' in OBS, select 'Stream'
7. Paste the RTMP ingest URL in the 'Server' field
8. On the Dashboard, copy your Stream Key
9. Paste it into the 'Stream Key' field in OBS
10. Save changes and hit 'Start Streaming'
11. Navigate back to the stream page to view your stream!

The Studio API and SDK can help you build an application that uses this capability. Check out [our docs](https://docs.livepeer.studio/guides/live/create-a-livestream) to learn more or start building with the [SDK](https://livepeerjs.org/). 

   
# Other livestreaming features

**Video Playback**

In order to playback a livestream with the playbackURL, a video player has to be used that supports HLS format. Livepeer Studio has a video player included in the SDK and we have an easy to embed player in our [documentation.](https://docs.livepeer.studio/guides/playback-a-video-stream)
   
**Recording**
   
You can record a livestream either throught the dashboard, SDK or the API.[Check out our docs](https://docs.livepeer.studio/guides/live/record-a-livestream) for more information.

**Multistreaming**

Livepeer Studio has the ability to multistream by pushing the livestream to multiple ingest points of other targets such as Twitch, YouTube and many others.


<Quiz id={"7bfm6"} />


</Section>

<Section name="4. Minting Videos" description="Introduction to Mint NFT videos">

# Minting Video NFTs
Livepeer Studio has a step-by-step guide for minting video NFTs using the Video NFT SDK or creating your own transaction.

 🌿 [Minting Video Guide](https://docs.livepeer.studio/guides/mint-a-video-nft)

</Section>

<Section name="5. Using Livepeer Studio" description="Introduction Using Livepeer Studio">

# Using Livepeer Studio in your project

 🗝 [Create an API key](https://docs.livepeer.studio/quickstart)

 🖥 [Dashboard](https://livepeer.studio/dashboard)

🧰 [SDK](https://livepeerjs.org/)

 🛠 [API](https://docs.livepeer.studio/category/api)

</Section>

<Section name="Livepeer Studio Resources" description="Additional Resources">

# Livepeer Studio Resources

### [Quickstart](https://docs.livepeer.studio/quickstart)

Get an API key and start building with Livepeer Studio.

### [Stream via OBS](https://docs.livepeer.studio/guides/live/stream-via-obs)

Using [OBS](https://obsproject.com/) software for livestreaming.

### [In-browser Streaming](https://docs.livepeer.studio/guides/live/stream-from-the-browser)

Using Livepeer Studio's [WebRTMP SDK](https://github.com/livepeer/webrtmp-sdk) from in-browser livestreams.

### [Support Matrix](https://docs.livepeer.studio/reference/support-matrix)

Descriptions and highlights of some of Livepeer Studio's capabilities.

### [Example Applications](https://docs.livepeer.studio/reference/examples)

Example of applications that incorporated Livepeer Studio.

### [Discord](https://discord.gg/xVYJxEr3)

Join the Livepeer Studio Community

</Section>