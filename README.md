# Download_videos
You can download any youtube videos 
just install Spotdl repository to start
install vs code software 
then install python
then just paste this code in vs code software 
import youtube_dl


def run():
    video_url = input("please enter youtube video url:")
    video_info = youtube_dl.YoutubeDL().extract_info(
        url=video_url, download=False
    )
    filename = f"{video_info['title']}.mp3"
    options = {
        'format': 'bestaudio/best',
        'keepvideo': False,
        'outtmpl': filename,
    }

    with youtube_dl.YoutubeDL(options) as ydl:
        ydl.download([video_info['webpage_url']])

    print("Download complete... {}".format(filename))


if __name__ == '__main__':
    run()

then press run then provide link to download and just wait patiently 
i not creat this code i am just promoting other code for better usage.
Thank you 
