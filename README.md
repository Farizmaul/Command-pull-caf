# Command-pull qcacld 3.0
git remote add qcacld-3.0 https://source.codeaurora.org/quic/la/platform/vendor/qcom-opensource/wlan/qcacld-3.0
git fetch qcacld-3.0 TAG
git merge -s ours --no-commit --allow-unrelated-histories FETCH_HEAD
git read-tree --prefix=drivers/staging/qcacld-3.0 -u FETCH_HEAD

git remote add fw-api https://source.codeaurora.org/quic/la/platform/vendor/qcom-opensource/wlan/fw-api
git remote add qca-wifi-host-cmn https://source.codeaurora.org/quic/la/platform/vendor/qcom-opensource/wlan/qca-wifi-host-cmn

git remote add audio-kernel https://source.codeaurora.org/quic/la/platform/vendor/opensource/audio-kernel
git merge -s ours --no-commit --allow-unrelated-histories FETCH_HEAD
git read-tree --prefix=techpack/audio -u FETCH_HEAD

git remote add camera-kernel https://source.codeaurora.org/quic/la/platform/vendor/opensource/camera-kernel
git remote add data-kernel https://source.codeaurora.org/quic/la/platform/vendor/qcom-opensource/data-kernel
git remote add display-drivers https://source.codeaurora.org/quic/la/platform/vendor/opensource/display-drivers
git remote add video-drivers https://source.codeaurora.org/quic/la/platform/vendor/opensource/video-driver
git remote add kernel https://source.codeaurora.org/quic/la/kernel/msm-4.19

# Command-upstream
