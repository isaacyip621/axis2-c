# Licensed to the Apache Software Foundation (ASF) under one or more
# contributor license agreements.  See the NOTICE file distributed with
# this work for additional information regarding copyright ownership.
# The ASF licenses this file to You under the Apache License, Version 2.0
# (the "License"); you may not use this file except in compliance with
# the License.  You may obtain a copy of the License at
# 
#   http://www.apache.org/licenses/LICENSE-2.0
# 
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
prgbindir=$(bindir)
prgbin_PROGRAMS = axis2_tcp_server
SUBDIRS =
AM_CFLAGS = -g 
axis2_tcp_server_SOURCES = tcp_server_main.c 

axis2_tcp_server_LDADD   =  $(LDFLAGS) \
		             $(top_builddir)/src/core/transport/http/common/libaxis2_http_common.la \
			     $(top_builddir)/axiom/src/om/libaxis2_axiom.la \
			     $(top_builddir)/util/src/libaxutil.la \
			     $(top_builddir)/axiom/src/parser/$(WRAPPER_DIR)/libaxis2_parser.la \
                             $(top_builddir)/src/core/description/libaxis2_description.la \
			     $(top_builddir)/src/core/deployment/libaxis2_deployment.la \
			     $(top_builddir)/src/core/context/libaxis2_context.la \
			     $(top_builddir)/src/core/clientapi/libaxis2_clientapi.la \
			     $(top_builddir)/src/core/engine/libaxis2_engine.la \
			     $(top_builddir)/src/core/transport/tcp/sender/libaxis2_tcp_sender.la \
			     $(top_builddir)/src/core/transport/tcp/receiver/libaxis2_tcp_receiver.la \
			     $(top_builddir)/neethi/src/libneethi.la

INCLUDES =  -I$(top_builddir)/include \
            -I$(top_builddir)/src/core/description\
            -I$(top_builddir)/src/core/context \
            -I$(top_builddir)/src/core/deployment\
            -I$(top_builddir)/src/core/phaseresolver \
            -I$(top_builddir)/src/core/engine \
            -I$(top_builddir)/util/include \
            -I../.. \
            -I$(top_builddir)/axiom/include
