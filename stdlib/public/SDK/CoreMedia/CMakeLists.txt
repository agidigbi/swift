add_swift_library(swiftCoreMedia ${SWIFT_SDK_OVERLAY_LIBRARY_BUILD_TYPES} IS_SDK_OVERLAY
  CoreMedia.swift
  CMTime.swift
  CMTimeRange.swift

  TARGET_SDKS OSX IOS IOS_SIMULATOR TVOS TVOS_SIMULATOR
  SWIFT_MODULE_DEPENDS Dispatch CoreAudio CoreGraphics Foundation
  SWIFT_MODULE_DEPENDS_OSX AppKit
  FRAMEWORK_DEPENDS CoreMedia)

