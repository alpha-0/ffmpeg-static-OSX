## FFmpeg Static Builder
####  For macOS with Intel Processor (Test on VM with macOS 13.6)

#### Include Last Versions of x264 | x265 | AV1 | FFmpeg…


```
./configure --extra-version=fanservice-"$(date +"%Y-%m-%d")" --extra-cflags="-fno-stack-check" --cc=/usr/bin/clang \
 --host-ldflags="-Wl,-ld_classic" --enable-pthreads --enable-postproc --enable-runtime-cpudetect \
 --pkg_config='pkg-config --static' --enable-nonfree --enable-gpl --enable-version3 --prefix=${TARGET} \
 --disable-ffplay --disable-ffprobe --disable-debug --disable-doc --enable-avfilter --enable-avisynth --enable-filters \
 --enable-libopus --enable-libtheora --enable-libvorbis --enable-libspeex --enable-libmp3lame --enable-libfdk-aac --enable-encoder=aac \
 --enable-libtwolame --enable-libopencore_amrnb --enable-libopencore_amrwb --enable-libgsm \
 --enable-libxvid --enable-libopenh264 --enable-libx264 --enable-libx265 --enable-libvpx \
 --enable-libaom --enable-libsvtav1 --enable-libdav1d --enable-librav1e \
 --enable-libfreetype --enable-libfribidi --enable-libass --enable-libsrt --enable-libfontconfig \
 --enable-libbluray --enable-bzlib --enable-zlib --enable-lzma --enable-libsnappy --enable-libopenjpeg --enable-libwebp \
 --enable-opengl --enable-opencl --enable-openal --enable-libzimg --enable-openssl --enable-librtmp  --enable-muxer=mp4
```

#### How Use :

##### =-> Download & Build :
```
cd ~/Desktop && git clone https://github.com/alpha-0/ffmpeg-static-OSX.git && \
chmod 755 ~/Desktop/ffmpeg-static-OSX/ffmpeg-static-OSX-with-hdr10plus.command  && \
~/Desktop/ffmpeg-static-OSX/ffmpeg-static-OSX-with-hdr10plus.command
```

#### Result :

##### =-> On Successfully Build :
`ffmpeg static binary will be copied on Desktop`

##### x-> On Error Build :
`Please Report with log to`
https://github.com/alpha-0/ffmpeg-static-OSX/issues

