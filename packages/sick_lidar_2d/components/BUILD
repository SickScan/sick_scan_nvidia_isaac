"""
Copyright 2019, SICK AG, Waldkirch

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http ://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
"""

load("@com_nvidia_isaac//engine/build:isaac.bzl", "isaac_cc_library", "isaac_cc_module", "isaac_component")

isaac_cc_library(
    name = "sick_lidar_2d",
    visibility = ["//visibility:public"],
    srcs = [
        "TiM5xxFamily.cpp",
        "SSBL_Wrapper.cpp"
    ],
    hdrs = [
        "SickIsaacLidar2D.hpp"
    ],
    deps = [
        "@com_sickag_ssbl//:ssbl",
        "@com_nvidia_isaac//engine/alice",
        "@com_nvidia_isaac//engine/core",
        "@com_nvidia_isaac//messages",
    ],
    copts = [
		"-Iexternal/com_sickag_ssbl/Components",
		"-Iexternal/com_sickag_ssbl/include",
    ],
)


