# SPDX-License-Identifier: MIT

if(CONFIG_BOARD_TOTEM_LEFT)
  board_runner_args(jlink "--device=nRF52840_xxAA" "--speed=4000")
  include(${ZEPHYR_BASE}/boards/common/nrfjprog.board.cmake)
  include(${ZEPHYR_BASE}/boards/common/jlink.board.cmake)
endif()

if(CONFIG_BOARD_TOTEM_RIGHT)
  board_runner_args(jlink "--device=nRF52840_xxAA" "--speed=4000")
  include(${ZEPHYR_BASE}/boards/common/nrfjprog.board.cmake)
  include(${ZEPHYR_BASE}/boards/common/jlink.board.cmake)
endif()
