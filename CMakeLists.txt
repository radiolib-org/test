cmake_minimum_required(VERSION 3.13)

file(GLOB_RECURSE ESP_SOURCES
  "src/*.*"
)

idf_component_register(
  SRCS ${ESP_SOURCES} 
  INCLUDE_DIRS . src 
)

