#
# Copyright 2019, Data61, CSIRO (ABN 41 687 119 230)
#
# SPDX-License-Identifier: BSD-2-Clause
#

cmake_minimum_required(VERSION 3.7.2)

if("${APP}" STREQUAL "susan")

    SusanRumprunPackages(susan_external rumprun_toplevel_support)
    CreateRumprunBakeCommand(susan RUMP_TARGETS susan_external)

endif()
