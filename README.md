https://chatgpt.com/share/e/ee58606f-4d50-4c76-bd97-60bce0e5637a

START_TIMESTAMP=$(date -u -d '5 minutes ago' +"%Y-%m-%dT%H:%M:%SZ")

aws kinesis-video-archived-media get-hls-streaming-session-url \
    --endpoint-url https://your-data-endpoint \
    --stream-name your-stream-name \
    --playback-mode LIVE_REPLAY \
    --hls-fragment-selector "{\"FragmentSelectorType\": \"SERVER_TIMESTAMP\", \"TimestampRange\": {\"StartTimestamp\": \"$START_TIMESTAMP\"}}" \
    --region ap-south-1
