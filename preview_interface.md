```html
<!-- Event Type Switcher -->
<div class="mb-4">
    <label for="event-type-switcher" class="text-sm font-medium text-slate-600 mr-2">Chọn loại sự kiện:</label>
    <select id="event-type-switcher" onchange="switchEventView(this.value)" class="bg-white border border-slate-300 rounded-md shadow-sm px-3 py-2 text-sm focus:outline-none focus:ring-1 focus:ring-blue-500 focus:border-blue-500">
        <option value="product-interest-event-view" selected>Sự kiện quan tâm sản phẩm</option>
        <option value="order-event-view">Sự kiện đơn hàng</option>
        <option value="loyalty-event-view">Sự kiện Loyalty</option>
        <option value="coupon-event-view">Sự kiện Coupon</option>
        <option value="livechat-event-view">Sự kiện Livechat</option>
    </select>
</div>

<div id="event-views-container">
    <!-- View 1: Product Interest Event (Original Content) -->
    <div id="product-interest-event-view" class="event-view">
        <!-- Lead Event Section -->
        <div id="global-lead-event" class="mb-6 w-full -mx-6 px-6">
            <!-- Collapsible Content -->
            <div id="leadEventTimeline" class="bg-white rounded-b-lg overflow-hidden">
                <!-- Top Section: Lead Event Header -->
                <div
                    class="mb-5 bg-blue-50 border border-blue-200 rounded-lg p-3 flex items-start gap-3 shadow-sm relative overflow-hidden">
                    <div
                        class="absolute right-0 top-0 bottom-0 w-24 bg-gradient-to-l from-blue-100/50 to-transparent pointer-events-none">
                    </div>
                    <div
                        class="w-10 h-10 rounded-full bg-white shadow-sm flex items-center justify-center text-blue-600 shrink-0 border border-blue-100/50 z-10">
                        <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M13 10V3L4 14h7v7l9-11h-7z"></path>
                        </svg>
                    </div>
                    <div class="z-10 flex-1">
                        <div
                            class="text-[12px] text-blue-500 font-semibold mb-0.5 uppercase tracking-wide">
                            Sự kiện tạo lead</div>
                        <div class="text-[14px] font-bold text-[#1b3da1] leading-tight">Lead khách hàng
                            vào từ quảng cáo</div>
                    </div>
                </div>

                <!-- Content Section: 2 Columns -->
                <div class="p-6 grid grid-cols-2 gap-8">
                    <!-- Left Column: Hành trình xét tuyển -->
                    <div>
                        <div class="flex items-center gap-2 mb-4">
                            <svg class="w-4 h-4 text-slate-500" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M12 2C6.5 2 2 6.5 2 12s4.5 10 10 10 10-4.5 10-10S17.5 2 12 2zm4.2 14.2L11 13V7h1.5v5.2l4.5 2.7-.8 1.3z" />
                            </svg>
                            <h4 class="text-[13px] font-bold text-slate-700">Hành trình xét tuyển</h4>
                        </div>
                        <div class="relative pl-5 border-l-2 border-slate-200 ml-2 flex flex-col gap-4">
                            <!-- Timeline Item 1 -->
                            <div class="relative">
                                <div class="absolute -left-[31px] top-0 w-8 h-8 rounded-full bg-indigo-600 flex items-center justify-center text-white shadow-sm ring-4 ring-white">
                                    <svg class="w-3.5 h-3.5" fill="currentColor" viewBox="0 0 24 24">
                                        <circle cx="12" cy="12" r="10"/>
                                    </svg>
                                </div>
                                <div class="pl-2">
                                    <div class="text-[12px] font-bold text-slate-800">Điền form nhận tư vấn</div>
                                    <div class="text-[11px] text-slate-500 mt-0.5">14:00 Hôm nay</div>
                                </div>
                            </div>

                            <!-- Timeline Item 2 -->
                            <div class="relative">
                                <div class="absolute -left-[31px] top-0 w-8 h-8 rounded-full bg-blue-600 flex items-center justify-center text-white shadow-sm ring-4 ring-white">
                                    <svg class="w-3.5 h-3.5" fill="currentColor" viewBox="0 0 24 24">
                                        <circle cx="12" cy="12" r="10"/>
                                    </svg>
                                </div>
                                <div class="pl-2">
                                    <div class="text-[12px] font-bold text-slate-800">Chuyên viên đã tư vấn</div>
                                    <div class="text-[11px] text-slate-500 mt-0.5">15:30 Hôm nay (Zalo Call)</div>
                                </div>
                            </div>

                            <!-- Timeline Item 3 -->
                            <div class="relative">
                                <div class="absolute -left-[31px] top-0 w-8 h-8 rounded-full bg-teal-500 flex items-center justify-center text-white shadow-sm ring-4 ring-white">
                                    <svg class="w-3.5 h-3.5" fill="currentColor" viewBox="0 0 24 24">
                                        <circle cx="12" cy="12" r="10"/>
                                    </svg>
                                </div>
                                <div class="pl-2">
                                    <div class="text-[12px] font-bold text-slate-800">Phụ huynh nộp hồ sơ</div>
                                    <div class="text-[11px] text-slate-500 mt-0.5">Vừa xong (Online)</div>
                                </div>
                            </div>

                            <!-- Timeline Item 4 -->
                            <div class="relative">
                                <div class="absolute -left-[31px] top-0 w-8 h-8 rounded-full bg-slate-400 flex items-center justify-center text-white shadow-sm ring-4 ring-white">
                                    <svg class="w-3.5 h-3.5" fill="currentColor" viewBox="0 0 24 24">
                                        <circle cx="12" cy="12" r="10"/>
                                    </svg>
                                </div>
                                <div class="pl-2">
                                    <div class="text-[12px] font-bold text-slate-800">Xác nhận nhập học</div>
                                    <div class="text-[11px] text-slate-500 mt-0.5">Đang chờ duyệt</div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Right Column: Nguyện vọng đăng ký & Hồ sơ đã nộp -->
                    <div class="flex flex-col gap-6">
                        <!-- Nguyện vọng đăng ký -->
                        <div>
                            <div class="flex items-center gap-2 mb-3">
                                <svg class="w-4 h-4 text-slate-500" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M12 2L1 7l11 5 9-4.09V17h2V7L12 2z" />
                                </svg>
                                <h4 class="text-[13px] font-bold text-slate-700">Nguyện vọng đăng ký</h4>
                            </div>
                            <div class="text-[13px] font-bold text-[#1b3da1] mb-1">Chương trình Cao đẳng Công nghệ Thông tin</div>
                            <div class="text-[12px] text-slate-600 mb-1">Hình thức: <span class="font-medium text-slate-800">Xét tuyển học bạ THPT</span></div>
                            <div class="text-[12px] font-bold text-amber-500">Trạng thái: Đang chờ duyệt hồ sơ</div>
                        </div>

                        <!-- Hồ sơ đã nộp -->
                        <div>
                            <div class="flex items-center gap-2 mb-3">
                                <svg class="w-4 h-4 text-slate-500" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M14 2H6c-1.1 0-1.99.9-1.99 2L4 20c0 1.1.89 2 1.99 2H18c1.1 0 2-.9 2-2V8l-6-6z" />
                                </svg>
                                <h4 class="text-[13px] font-bold text-slate-700">Hồ sơ đã nộp</h4>
                            </div>
                            <ul class="text-[12px] text-slate-600 flex flex-col gap-2">
                                <li class="flex items-start gap-2">
                                    <span class="text-emerald-500 mt-0.5"><svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                                    </svg></span>
                                    <div class="leading-tight">Căn cước công dân (Bản sao)</div>
                                </li>
                                <li class="flex items-start gap-2">
                                    <span class="text-emerald-500 mt-0.5"><svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                                    </svg></span>
                                    <div class="leading-tight">Học bạ THPT (Bản sao)</div>
                                </li>
                                <li class="flex items-start gap-2 opacity-50">
                                    <span class="text-slate-400 mt-0.5"><svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4m0 4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                                    </svg></span>
                                    <div class="leading-tight">Giấy chứng nhận tốt nghiệp tạm thời</div>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- View 2: Order Event -->
    <div id="order-event-view" class="event-view" style="display: none;">
        <div class="mb-6 w-full -mx-6 px-6">
            <div class="bg-white rounded-b-lg overflow-hidden">
                <!-- Top Section: Order Event Header -->
                <div class="mb-5 bg-red-50 border border-red-200 rounded-lg p-3 flex items-start gap-3 shadow-sm relative overflow-hidden">
                    <div class="w-10 h-10 rounded-full bg-white shadow-sm flex items-center justify-center text-red-600 shrink-0 border border-red-100/50 z-10">
                        <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M18.364 18.364A9 9 0 005.636 5.636m12.728 12.728A9 9 0 015.636 5.636m12.728 12.728L5.636 5.636"></path></svg>
                    </div>
                    <div class="z-10 flex-1">
                        <div class="text-[12px] text-red-500 font-semibold mb-0.5 uppercase tracking-wide">Sự kiện đơn hàng</div>
                        <div class="text-[14px] font-bold text-red-900 leading-tight">Đơn hàng bị khách từ chối</div>
                    </div>
                    <span class="text-xs font-bold text-red-600 bg-red-100 px-2 py-1 rounded-md">Rất cao</span>
                </div>

                <!-- Content Section: Order Details -->
                <div class="p-6">
                    <h4 class="text-[13px] font-bold text-slate-700 mb-3">Chi tiết đơn hàng #DH60567</h4>
                    <div class="grid grid-cols-2 gap-6">
                        <div>
                            <p class="text-sm text-slate-600 mb-1"><span class="font-semibold">Sản phẩm:</span> Một cưới (Seri) x2, sp 123 x1</p>
                            <p class="text-sm text-slate-600 mb-1"><span class="font-semibold">Tổng giá trị:</span> <span class="font-bold text-slate-800">80.508.621 VND</span></p>
                            <p class="text-sm text-slate-600"><span class="font-semibold">Thanh toán:</span> COD - Chưa thanh toán</p>
                        </div>
                        <div>
                            <p class="text-sm text-slate-600 mb-1"><span class="font-semibold">Giao hàng:</span> GHTK - <span class="text-red-600 font-medium">Khách từ chối nhận</span></p>
                            <p class="text-sm text-slate-600"><span class="font-semibold">Địa chỉ:</span> 12 lạc long quân, Thanh Hóa</p>
                        </div>
                    </div>
                    <div class="mt-4 pt-4 border-t border-slate-200">
                        <h4 class="text-[13px] font-bold text-slate-700 mb-2">Lịch sử đơn hàng (5)</h4>
                        <ul class="text-xs text-slate-500 space-y-1">
                            <li>#DH60561 - 27/06/25 - 3.833.744 VND - <span class="text-emerald-600">Thành công</span></li>
                            <li>#DH59902 - 15/05/25 - 2.100.000 VND - <span class="text-emerald-600">Thành công</span></li>
                            <li>#DH59123 - 01/04/25 - 5.500.000 VND - <span class="text-red-600">Đã hủy</span></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Placeholder for other views -->
    <div id="loyalty-event-view" class="event-view" style="display: none;"><div class="p-6 text-slate-500">Nội dung cho sự kiện Loyalty sẽ được hiển thị ở đây.</div></div>
    <div id="coupon-event-view" class="event-view" style="display: none;"><div class="p-6 text-slate-500">Nội dung cho sự kiện Coupon sẽ được hiển thị ở đây.</div></div>
    <div id="livechat-event-view" class="event-view" style="display: none;"><div class="p-6 text-slate-500">Nội dung cho sự kiện Livechat sẽ được hiển thị ở đây.</div></div>
</div>

<script>
    function switchEventView(viewId) {
        const views = document.querySelectorAll('.event-view');
        views.forEach(view => {
            view.style.display = 'none';
        });
        const activeView = document.getElementById(viewId);
        if (activeView) {
            activeView.style.display = 'block';
        }
    }
</script>
```
