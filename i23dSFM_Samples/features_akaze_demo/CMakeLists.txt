
ADD_DEFINITIONS(-DTHIS_SOURCE_DIR="${CMAKE_CURRENT_SOURCE_DIR}")

ADD_EXECUTABLE(i23dSFM_sample_akaze akaze_demo.cpp)
TARGET_LINK_LIBRARIES(i23dSFM_sample_akaze
  i23dSFM_image
  i23dSFM_features
  stlplus
  ${I23DSFM_LIBRARY_DEPENDENCIES})
SET_PROPERTY(TARGET i23dSFM_sample_akaze PROPERTY FOLDER I23dSFM/Samples)

ADD_EXECUTABLE( i23dSFM_main_computeAKAZE main_computeAKAZE.cpp )
TARGET_LINK_LIBRARIES( i23dSFM_main_computeAKAZE
  i23dSFM_image
  i23dSFM_features
  i23dSFM_system
  stlplus
  ${I23DSFM_LIBRARY_DEPENDENCIES})
SET_PROPERTY(TARGET i23dSFM_main_computeAKAZE PROPERTY FOLDER I23dSFM/Samples)

