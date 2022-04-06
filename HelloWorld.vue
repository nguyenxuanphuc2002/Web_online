<template>
  <div>
    <div id="user-div">
      <ul class="header">
        <li class="Header">BKExam</li>
        <li class="search">
          <input class="search-input" type="text" placeholder="Tìm kiếm" />
          <button class="ti-search btn-search"></button>
        </li>
        <li class="Name">
          Nguyen Xuan Phuc
          <button class="fa-solid fa-user btn-user"></button>
        </li>
        <li>
          <button class="fa-solid fa-bell noti-btn"></button>
        </li>
      </ul>
    </div>
    <div class="clear"></div>
    <div id="slidebar">
      <div class="overview">
        <button class="overview-btn js-overview-btn">
          <i class="ti-layout-grid2"></i> Tổng Quan
        </button>
      </div>
      <div class="schedule">
        <button class="schedule-btn">
          <i class="ti-calendar"></i> Lịch thi
        </button>
      </div>
      <div class="grades">
        <button class="grades-btn"><i class="ti-check"></i> Kết quả thi</button>
      </div>
      <div class="document">
        <button class="document-btn">
          <i class="fa-solid fa-file-lines"></i> Tài liệu
        </button>
      </div>
      <div class="settings">
        <button class="settings-btn">
          <i class="ti-settings"></i> Cài đặt
        </button>
      </div>
    </div>
    <div class="content-user"></div>
    <div class="content-overview js-content-overview">
      <div class="overview2 content-center">
        <ul>
          <li class="coming-sub">
            <h2>Môn thi sắp tới</h2>
            <button type="button">
              <div class="btn-sub">
                <ul>
                  <li class="sub">Kinh tế chính trị</li>
                  <ul>
                    <li class="date">Ngày thi : 23/03/2022</li>
                    <li class="date">Kíp 4 : 12h30 - 14h30</li>
                  </ul>
                  <li class="code-class">
                    120175 - Khoa học máy tinh K65 nhóm 1
                  </li>
                </ul>
              </div>
            </button>
          </li>
          <li class="point">
            <h2>Kết quả thi</h2>
            <button type="button">
              <div class="point-btn">
                <h2 class="sub">Vật lý đại cương 2</h2>
                <ul>
                  <li class="status content-point-btn">
                    Trạng thái : Đã nộp bài
                  </li>
                  <li class="result content-point-btn">Kết quả : -</li>
                </ul>
              </div>
            </button>
          </li>
          <li class="question">
            <h2 class="question-sub">Câu hỏi ôn tập</h2>
            <div class="ul1">
              <button type="button">
                <div class="list-question">
                  <p class="question1">
                    Thuật ngữ "Kinh tế chính trị được sử dụng đầu tiên khi nào"
                  </p>
                  <ul>
                    <li class="switch">A. 1610</li>
                    <li class="switch">B. 1615</li>
                    <li class="switch">C. 1620</li>
                    <li class="switch">D. 1625</li>
                  </ul>
                  <p class="sub-question">Kinh tế chính trị</p>
                  <p class="quanity">20 câu hỏi</p>
                </div>
              </button>
              <button type="button">
                <div class="list-question">
                  <p class="question1">
                    Thuật ngữ "Kinh tế chính trị được sử dụng đầu tiên khi nào"
                  </p>
                  <ul>
                    <li class="switch">A. 1610</li>
                    <li class="switch">B. 1615</li>
                    <li class="switch">C. 1620</li>
                    <li class="switch">D. 1625</li>
                  </ul>
                  <p class="sub-question">Kinh tế chính trị</p>
                  <p class="quanity">20 câu hỏi</p>
                </div>
              </button>
            </div>
          </li>
        </ul>
      </div>
      <div class="overview2 content-right">
        <button type="button" class="contet-right-btn">
          <div class="content-right-header">
            <p>Lịch thi sắp tới</p>
            <p style="" class="date">Ngày 17 tháng 03 năm 2022</p>
          </div>
          <div class="times">
            <ul>
              <li class="time">
                12:00 ---------------------------------------------
              </li>
              <li class="time">
                13:00 ---------------------------------------------
              </li>
              <li class="time">
                14:00 ---------------------------------------------
              </li>
              <li class="time">
                15:00 ---------------------------------------------
              </li>
              <li class="time">
                16:00 ---------------------------------------------
              </li>
              <li class="time">
                17:00 ---------------------------------------------
              </li>
              <li class="time">
                18:00 ---------------------------------------------
              </li>
              <li class="time">
                19:00 ---------------------------------------------
              </li>
              <li class="time">
                20:00 ---------------------------------------------
              </li>
              <li class="time">
                21:00 ---------------------------------------------
              </li>
            </ul>
          </div>
        </button>
      </div>
    </div>
    <div class="content-shedule"></div>
    <div class="content-grades"></div>
    <div class="content-document"></div>
    <div class="content-settings"></div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.clear {
  clear: both;
}
.content-overview.open {
  display: flex;
}
html {
}
#slidebar {
}
.header {
  width: 1446px;
  height: 100px;
  margin-top: 16px;
  display: flex;
  align-items: center;
  position: relative;
  min-width: calc(100%-32px);
}
.header li {
  display: inline;
}
.header .Header {
  width: 377px;
  height: 180px;
  font-family: "Poppins";
  font-style: normal;
  font-weight: 400;
  font-size: 40px;
  line-height: 180px;
  color: #3a3a3a;
  border-right: 2px solid #353535;
}
ul {
  list-style-type: none;
}
.header .search {
  width: 600px;
  height: 60;
  margin-left: 40px;
  color: #3a3a3a;
  padding: 12px 0;
  font-size: 20px;
}
.header .btn-search {
  width: 24px;
  height: 24px;
  font-size: large;
  border-style: none;
  border-color: #fff;
  background-color: #fff;
}
.btn-search:hover {
  opacity: 0.7;
  background-color: #353535;
  color: #fff;
}
.header .search-input {
  border-radius: 29px;
  border-color: #969696;
  width: 300px;
  padding-left: 12px;
}

.header .Name {
  font-family: "Poppins";
  font-style: normal;
  font-weight: 400;
  font-size: 23px;
  line-height: 60px;
  width: 362px;
  height: 60px;
  text-align: center;
  margin-left: 480px;
  color: #3a3a3a;
}
.header .btn-user {
  background-color: #fff;
  border-radius: 100%;
  border-style: none;
  font-size: large;
  padding: 12px;
}
.header .btn-user:hover {
  background-color: #d49eff;
  opacity: 0.7;
}
.header .noti-btn {
  border-style: none;
  background-color: #fff;
  font-size: large;
}
.noti-btn:hover {
  opacity: 0.6;
}
#slidebar {
  border-right: 2px solid #353535;
  width: 284px;
  height: 79vh;
  padding: 32px;
  font-size: 20px;
  margin-top: 40px;
  border-top: 2px solid #353535;
}
#slidebar .overview-btn,
#slidebar .schedule-btn,
#slidebar .grades-btn,
#slidebar .document-btn,
#slidebar .settings-btn {
  height: 56px;
  border: none;
  background-color: #fff;
  padding: 0 24px;
  font-size: 25px;
  margin-top: 8px;
}
#slidebar .overview-btn:hover,
#slidebar .schedule-btn:hover,
#slidebar .grades-btn:hover,
#slidebar .document-btn:hover,
#slidebar .settings-btn:hover {
  background-color: #d49eff;
  color: #5b1674;
  border-radius: 40px;
}
.content-overview {
  display: none;
  position: fixed;
  margin-top: -600px;
  left: 200px;
}
.overview2 {
  display: inline-block;
  float: left;
}
.coming-sub button {
  background-color: #fff;
  border-style: none;
}
.coming-sub button:hover {
  box-shadow: 0px 0px 10px rgba(58, 58, 58, 0.5);
  width: 736px;
  height: 140px;
  border-radius: 24px;
}
.content-center {
  margin-left: 100px;
  margin-top: 0;
  list-style-type: none;
}
.coming-sub .btn-sub {
  width: 736px;
  height: 140px;
  background: #ffffff;
  box-shadow: 0px 0px 10px rgba(58, 58, 58, 0.25);
  border-radius: 24px;
  border-color: #ffffff;
  text-align: left;
  display: flex;
  justify-content: left;
  align-items: center;
  line-height: 37.5px;
  font-family: "Poppins";
  font-style: normal;
  display: block;
}
.coming-sub h2 {
  font-size: 25px;
  padding-left: 32px;
  font-style: Bold;
  text-align: left;
}
.coming-sub .sub {
  font-weight: 600;
  font-size: 25px;
  line-height: 38px;
  color: #3a3a3a;
  font-style: Bold;
  padding-left: 32px;
  padding-top: 12px;
}
.coming-sub .date {
  display: inline;
  padding-right: 120px;
  font-family: "Poppins";
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
}
.coming-sub .code-class {
  padding-left: 32px;
  font-weight: 400;
  font-size: 20px;
}
.point button {
  background-color: #fff;
  border-style: none;
}
.point button:hover {
  box-shadow: 0px 0px 10px rgba(58, 58, 58, 0.5);
  width: 736px;
  height: 120px;
  border-radius: 24px;
}
.point > h2 {
  margin-top: 21px;
  padding-left: 32px;
  font-size: 25px;
  padding-left: 32px;
  font-style: Bold;
}
.point-btn {
  width: 736px;
  height: 120px;
  background: #ffffff;
  box-shadow: 0px 0px 10px rgba(58, 58, 58, 0.25);
  border-radius: 24px;
  line-height: 37.5px;
  border-color: #ffffff;
  font-family: "Poppins";
  font-style: normal;
  text-align: left;
}

.point-btn .sub {
  font-size: 25px;
  padding-left: 62px;
  padding-top: 24px;
  font-style: Bold;
  font-weight: 600;
}
.point-btn ul {
}
.point-btn .content-point-btn {
  display: inline;
  font-weight: 400;
  font-size: 20px;
}
.point-btn .status {
  padding-right: 116px;
  padding-left: 32px;
}
.question button {
  background-color: #fff;
  border-style: none;
}
.question button:hover {
  box-shadow: 0px 0px 10px rgba(58, 58, 58, 0.5);
  width: 360px;
  height: 160px;
  border-radius: 24px;
  margin-right: 20px;
}
.question .list-question {
  width: 360px;
  height: 160px;
  background: #ffffff;
  box-shadow: 0px 0px 10px rgba(58, 58, 58, 0.25);
  border-radius: 24px;
  line-height: 37.5px;
  font-size: 12px;
  display: inline-block;
  margin-right: 16px;
  text-align: left;
}

.question {
  margin-top: 20px;
  float: left;
}
.question .ul1 {
  padding: 0;
}
.question .question-sub {
  padding-left: 32px;
  font-weight: 600;
  font-size: Bold;
}
.question .switch {
  display: inline;
  padding-right: 100px;
  padding-left: 16px;
}
.list-question .question1 {
  padding-left: 32px;
  margin-bottom: -12px;
}
.list-question .sub-question {
  font-family: "Poppins";
  font-style: normal;
  font-weight: 600;
  font-size: 20px;
  line-height: 30px;
  margin-bottom: -8px;
  padding-left: 32px;
}
.list-question .quanity {
  padding-left: 32px;
  font-family: "Poppins";
  font-style: normal;
  font-weight: 600;
  font-size: 15px;
  line-height: 22px;
  color: #655aa6;
}
.content-right {
  width: 352px;
  height: 590px;
  box-shadow: 0 0 10px rgba(58, 58, 58, 0.25);
  margin-left: 20px;
  border-radius: 24px;
}

.content-right button:hover {
  width: 352px;
  height: 590px;
  box-shadow: 0 0 10px rgba(58, 58, 58, 0.5);
}
.content-right button {
  width: 352px;
  height: 590px;
  box-shadow: 0 0 10px rgba(58, 58, 58, 0.25);
  background-color: #fff;
  border-style: none;
  border-radius: 24px;
}
.content-right-header {
  text-align: left;
  padding-left: 12px;
  font-family: "Poppins";
  font-style: normal;
  font-weight: 400;
  font-size: 25px;
  line-height: 38px;
  text-decoration: none;
}
.content-right-header > p {
  padding-left: 26px;
}
.content-right-header .date {
  font-family: "Poppins";
  font-style: normal;
  font-weight: 400;
  font-size: 15px;
  line-height: 22px;
  margin-bottom: 41px;
}
.time {
  width: 36px;
  height: 23px;
  font-family: "Poppins";
  font-style: normal;
  font-weight: 400;
  font-size: 15px;
  line-height: 22px;
  margin-bottom: 20px;
  /* text-decoration: underline; */
  width: 280px;
  height: 23px;
  text-align: left;
}
.times {
  margin-left: 19px;
}
</style>
