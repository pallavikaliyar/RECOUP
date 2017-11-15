/*
 * Copyright (c) 2014, VUB - ETRO
 * All rights reserved.
 *
 * Redistribution and use in source and binary forms, with or without
 * modification, are permitted provided that the following conditions
 * are met:
 * 1. Redistributions of source code must retain the above copyright
 *    notice, this list of conditions and the following disclaimer.
 * 2. Redistributions in binary form must reproduce the above copyright
 *    notice, this list of conditions and the following disclaimer in the
 *    documentation and/or other materials provided with the distribution.
 * 3. Neither the name of the Institute nor the names of its contributors
 *    may be used to endorse or promote products derived from this software
 *    without specific prior written permission.
 *
 * THIS SOFTWARE IS PROVIDED BY THE INSTITUTE AND CONTRIBUTORS ``AS IS'' AND
 * ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
 * ARE DISCLAIMED.  IN NO EVENT SHALL THE INSTITUTE OR CONTRIBUTORS BE LIABLE
 * FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 * DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
 * OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
 * HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 * LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
 * OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
 * SUCH DAMAGE.
 *
 * This file is part of the Contiki operating system.
 */

/**
 * \file
 *         Header file for Secure and Robust Multicast RPL Forwarding' (SeRI)
 *
 * \author
 *         Pallavi Kaliyar
 */

#ifndef SeRI_H_
#define SeRI_H_

#include "contiki-conf.h"

#include <stdint.h>

#define SeRI_UNICAST_MODE      0


/*---------------------------------------------------------------------------*/
/* Configuration */
/*---------------------------------------------------------------------------*/

/* Fmin */
#ifdef SeRI_CONF_MIN_FWD_DELAY
#define SeRI_MIN_FWD_DELAY SeRI_CONF_MIN_FWD_DELAY
#else
#define SeRI_MIN_FWD_DELAY 4
#endif

/* Max Spread */
#ifdef SeRI_CONF_MAX_SPREAD
#define SeRI_MAX_SPREAD SeRI_CONF_MAX_SPREAD
#else
#define SeRI_MAX_SPREAD 4
#endif

/*---------------------------------------------------------------------------*/
/* Stats datatype */
/*---------------------------------------------------------------------------*/
struct seri_stats {
    UIP_MCAST6_STATS_DATATYPE seri_fwd_uncst;  /* Forwarded by us with LL Unicast*/
};

#endif /* SeRI_H_ */
