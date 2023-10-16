# Description:
#   OpenCV libraries for video/image processing on Linux

licenses(["notice"])  # BSD license

exports_files(["LICENSE"])

OPENCVWASM_BUILD_PATH = "build_wasm/"

OPENCVWASM_INSTALL_PATH = "install/"

cc_library(
    name = "opencv",
    srcs = glob([ OPENCVWASM_BUILD_PATH + "lib/*.a" ]),
    hdrs = glob([
        OPENCVWASM_INSTALL_PATH + "include/opencv4/opencv2/**/*.h*",
    ]),
    includes = [
        OPENCVWASM_INSTALL_PATH + "include/opencv4/",
    ],
    strip_include_prefix = OPENCVWASM_INSTALL_PATH,
    visibility = ["//visibility:public"],
)
