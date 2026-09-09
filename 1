async function onRequest(context, request) {
    return request;
}

async function onResponse(context, request, response) {
    try {
        // 精准匹配完整接口地址
        const targetUrl = "https://3h-wolrdcup-memapi.bdhzrs.com/v1/api/activity/selfMediaStar/canApply";
        if (request.url !== targetUrl) {
            // 不是目标接口直接跳过
            return response;
        }

        console.log("✅命中目标接口：", request.url);

        // 兼容大小写获取content-type
        const ct = (response.headers["Content-Type"] || response.headers["content-type"] || "").toLowerCase();
        if (!ct.includes("application/json")) {
            console.log("❌该接口不是JSON响应");
            return response;
        }

        // 解析响应
        const obj = JSON.parse(response.body);
        console.log("原始 can_apply =", obj.data?.can_apply);

        // 修改false为true
        if(obj.data && obj.data.can_apply === false){
            obj.data.can_apply = true;
            console.log("🎉修改 can_apply => true");
        }

        // 回写响应体
        response.body = JSON.stringify(obj);
        console.log("修改后的响应：", response.body);

    } catch (err) {
        console.error("❌脚本报错：", err);
    }
    return response;
}