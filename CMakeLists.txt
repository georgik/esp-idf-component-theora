
idf_component_register(
    SRCS
        "theora/lib/fragment.c"
        "theora/lib/collect.c"
        "theora/lib/encapiwrapper.c"
        "theora/lib/fdct.c"
        "theora/lib/rate.c"
        "theora/lib/info.c"
        "theora/lib/decinfo.c"
        "theora/lib/decode.c"
        "theora/lib/dequant.c"
        "theora/lib/encode.c"
        "theora/lib/huffenc.c"
        "theora/lib/mathops.c"
        "theora/lib/internal.c"
        "theora/lib/encoder_disabled.c"
        "theora/lib/enquant.c"
        "theora/lib/apiwrapper.c"
        "theora/lib/mcenc.c"
        "theora/lib/decapiwrapper.c"
        "theora/lib/encinfo.c"
        "theora/lib/tokenize.c"
        "theora/lib/bitpack.c"
        "theora/lib/idct.c"
        "theora/lib/quant.c"
        "theora/lib/huffdec.c"

        # Patch of oc_state_loop_filter_frag_rows_c signature to signed char _bv[256] - to match header
        #"theora/lib/state.c"
        "src/lib/state.c"

        # Patch of oc_cost_inter_nomv signature to rd_scale[5]
        #"theora/lib/analyze.c"
        "src/lib/analyze.c"

        # Pach of oc_enc_frag_sub_128_c to _diff[64]
        # "theora/lib/encfrag.c"
        "src/lib/encfrag.c"

    INCLUDE_DIRS
        "theora/include"
        "theora/lib"
    REQUIRES
        georgik__ogg
)


