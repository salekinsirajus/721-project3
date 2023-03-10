set(
        softfloat_hdrs
        internals.h
        primitives.h
        softfloat.h
        softfloat_types.h
        platform.h
        specialize.h
)

set(
        softfloat_c_srcs
        f32_add.c
        f32_div.c
        f32_eq.c
        f32_eq_signaling.c
        f32_isSignalingNaN.c
        f32_le.c
        f32_le_quiet.c
        f32_lt.c
        f32_lt_quiet.c
        f32_mulAdd.c
        f32_mul.c
        f32_rem.c
        f32_roundToInt.c
        f32_sqrt.c
        f32_sub.c
        f32_to_f64.c
        f32_to_i32.c
        f32_to_i32_r_minMag.c
        f32_to_i64.c
        f32_to_i64_r_minMag.c
        f32_to_ui32.c
        f32_to_ui32_r_minMag.c
        f32_to_ui64.c
        f32_to_ui64_r_minMag.c
        f32_classify.c
        f64_add.c
        f64_div.c
        f64_eq.c
        f64_eq_signaling.c
        f64_isSignalingNaN.c
        f64_le.c
        f64_le_quiet.c
        f64_lt.c
        f64_lt_quiet.c
        f64_mulAdd.c
        f64_mul.c
        f64_rem.c
        f64_roundToInt.c
        f64_sqrt.c
        f64_sub.c
        f64_to_f32.c
        f64_to_i32.c
        f64_to_i32_r_minMag.c
        f64_to_i64.c
        f64_to_i64_r_minMag.c
        f64_to_ui32.c
        f64_to_ui32_r_minMag.c
        f64_to_ui64.c
        f64_to_ui64_r_minMag.c
        f64_classify.c
        i32_to_f32.c
        i32_to_f64.c
        i64_to_f32.c
        i64_to_f64.c
        s_add128.c
        s_add192.c
        s_addMagsF32.c
        s_addMagsF64.c
        s_countLeadingZeros32.c
        s_countLeadingZeros64.c
        s_countLeadingZeros8.c
        s_eq128.c
        s_estimateDiv128To64.c
        s_estimateSqrt32.c
        s_le128.c
        s_lt128.c
        s_mul128By64To192.c
        s_mul128To256.c
        s_mul64To128.c
        s_mulAddF32.c
        s_mulAddF64.c
        s_normRoundPackToF32.c
        s_normRoundPackToF64.c
        s_normSubnormalF32Sig.c
        s_normSubnormalF64Sig.c
        softfloat_state.c
        s_roundPackToF32.c
        s_roundPackToF64.c
        s_roundPackToI32.c
        s_roundPackToI64.c
        s_roundPackToUI32.c
        s_roundPackToUI64.c
        s_shift128ExtraRightJam.c
        s_shift128RightJam.c
        s_shift32RightJam.c
        s_shift64ExtraRightJam.c
        s_shift64RightJam.c
        s_shortShift128ExtraRightJam.c
        s_shortShift128Left.c
        s_shortShift128Right.c
        s_shortShift192Left.c
        s_shortShift32Right1Jam.c
        s_shortShift64ExtraRightJam.c
        s_shortShift64RightJam.c
        s_sub128.c
        s_sub192.c
        s_subMagsF32.c
        s_subMagsF64.c
        ui32_to_f32.c
        ui32_to_f64.c
        ui64_to_f32.c
        ui64_to_f64.c
        softfloat_raiseFlags.c
        s_commonNaNToF32UI.c
        s_commonNaNToF64UI.c
        s_f32UIToCommonNaN.c
        s_f64UIToCommonNaN.c
        s_isSigNaNF32UI.c
        s_isSigNaNF64UI.c
        s_propagateNaNF32UI.c
        s_propagateNaNF64UI.c
)

add_library(
        softfloat STATIC
        ${softfloat_c_srcs}
        ${softfloat_hdrs}
)

target_include_directories(softfloat PUBLIC .)
