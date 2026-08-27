---
hide:
  - navigation
  - toc
---

<div class="landing-page">
  <section class="landing-hero">
    <div class="landing-hero__content">
      <p class="landing-eyebrow">DATA ENGINEERING · FIELD NOTES</p>
      <h1>Kiến trúc dữ liệu,<br><span>được giải thích từ gốc.</span></h1>
      <p class="landing-hero__lead">
        Những ghi chú cô đọng về cách các hệ thống dữ liệu vận hành — bắt đầu
        từ Apache Airflow, từ bài toán thực tế đến kiến trúc bên trong.
      </p>
      <div class="landing-actions">
        <a class="landing-button landing-button--primary" href="airflow/architecture/">
          Bắt đầu với Airflow <span aria-hidden="true">→</span>
        </a>
        <a class="landing-button landing-button--secondary" href="#noi-dung">
          Xem nội dung
        </a>
      </div>
    </div>

    <div class="landing-hero__visual" aria-label="Minh họa một data pipeline được điều phối">
      <div class="pipeline-window">
        <div class="pipeline-window__bar">
          <span></span><span></span><span></span>
          <strong>daily_data_pipeline</strong>
        </div>
        <div class="pipeline-status">
          <span class="pipeline-status__dot"></span>
          <span>Pipeline đang hoạt động</span>
          <small>@daily</small>
        </div>
        <div class="pipeline-flow">
          <div class="pipeline-node">
            <span>01</span>
            <strong>Extract</strong>
            <small>success</small>
          </div>
          <i aria-hidden="true"></i>
          <div class="pipeline-node pipeline-node--active">
            <span>02</span>
            <strong>Transform</strong>
            <small>running</small>
          </div>
          <i aria-hidden="true"></i>
          <div class="pipeline-node pipeline-node--pending">
            <span>03</span>
            <strong>Load</strong>
            <small>queued</small>
          </div>
        </div>
        <div class="pipeline-meta">
          <span><b>3</b> tasks</span>
          <span><b>1</b> running</span>
          <span><b>02:00</b> schedule</span>
        </div>
      </div>
    </div>
  </section>

  <section class="landing-principles" aria-label="Định hướng nội dung">
    <p>Từ vấn đề thực tế</p>
    <span aria-hidden="true">→</span>
    <p>Đến khái niệm cốt lõi</p>
    <span aria-hidden="true">→</span>
    <p>Đi sâu vào kiến trúc</p>
  </section>

  <section class="landing-section" id="noi-dung">
    <div class="landing-section__heading">
      <p class="landing-eyebrow">CHỦ ĐỀ ĐẦU TIÊN</p>
      <h2>Hiểu Airflow từ nhu cầu điều phối</h2>
      <p>
        Bài viết đi từ Bash và Cron đến những khái niệm nền tảng, sau đó mở
        rộng vào Scheduler, HA Scheduler, Critical Section và Executor.
      </p>
    </div>

    <div class="topic-grid">
      <a class="topic-card" href="airflow/architecture/#tai-sao-can-airflow">
        <span class="topic-card__number">01</span>
        <p class="topic-card__label">BÀI TOÁN</p>
        <h3>Tại sao cần Airflow?</h3>
        <p>Khi nào Bash và Cron là đủ, và khi nào workflow cần một orchestrator?</p>
        <strong>Đọc nội dung <span aria-hidden="true">→</span></strong>
      </a>

      <a class="topic-card" href="airflow/architecture/#nhung-khai-niem-nen-tang">
        <span class="topic-card__number">02</span>
        <p class="topic-card__label">NỀN TẢNG</p>
        <h3>Những khái niệm cốt lõi</h3>
        <p>DAG, Task, Task Instance, Schedule và Dependency trong một workflow.</p>
        <strong>Đọc nội dung <span aria-hidden="true">→</span></strong>
      </a>

      <a class="topic-card topic-card--featured" href="airflow/architecture/#cac-component-trong-airflow">
        <span class="topic-card__number">03</span>
        <p class="topic-card__label">KIẾN TRÚC</p>
        <h3>Cách Airflow vận hành</h3>
        <p>Scheduler, scheduling loop, HA, Critical Section, Pool và Executor.</p>
        <strong>Khám phá kiến trúc <span aria-hidden="true">→</span></strong>
      </a>
    </div>
  </section>

  <section class="learning-path">
    <div class="learning-path__intro">
      <p class="landing-eyebrow">LỘ TRÌNH ĐỌC</p>
      <h2>Một mạch kiến thức liền lạc</h2>
      <p>
        Mỗi phần nối tiếp phần trước, giúp bạn hiểu lý do một thành phần tồn tại
        trước khi tìm hiểu cách nó hoạt động.
      </p>
    </div>

    <ol class="learning-steps">
      <li>
        <span>01</span>
        <div><strong>Bash &amp; Cron</strong><small>Điểm khởi đầu của việc điều phối</small></div>
      </li>
      <li>
        <span>02</span>
        <div><strong>DAG &amp; Task</strong><small>Mô hình hóa workflow và dependency</small></div>
      </li>
      <li>
        <span>03</span>
        <div><strong>Scheduler &amp; Executor</strong><small>Cơ chế lập lịch và thực thi</small></div>
      </li>
      <li>
        <span>04</span>
        <div><strong>HA &amp; Critical Section</strong><small>Mở rộng an toàn với nhiều Scheduler</small></div>
      </li>
    </ol>
  </section>

  <section class="landing-cta">
    <div>
      <p class="landing-eyebrow">BẮT ĐẦU KHÁM PHÁ</p>
      <h2>Đi sâu vào kiến trúc Apache Airflow</h2>
      <p>Từ một pipeline Bash đơn giản đến cách Airflow điều phối hàng nghìn task.</p>
    </div>
    <a class="landing-button landing-button--light" href="airflow/architecture/">
      Đọc bài viết <span aria-hidden="true">→</span>
    </a>
  </section>
</div>
