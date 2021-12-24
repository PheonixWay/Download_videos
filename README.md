# Download_videos
1.You can download any youtube videos 
2.just install Spotdl repository to start
3.install vs code software 
4.then install python
5.then just paste this code in vs code software 
6.import youtube_dl


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

7.then press run then provide link to download and just wait patiently 
8.i not creat this code i am just promoting other code for better usage.
9.Thank you 
