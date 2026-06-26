<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Калькулятор дверей</title>
  <style>
    * { box-sizing: border-box; font-family: system-ui, sans-serif; }
    body { background: #f5f7fa; padding: 20px; display: flex; justify-content: center; }
    .app { max-width: 1100px; width: 100%; background: white; padding: 24px; border-radius: 20px; box-shadow: 0 8px 24px rgba(0,0,0,0.1); }
    h1 { font-size: 24px; margin-top: 0; margin-bottom: 24px; }
    
    /* ДВЕ КОЛОНКИ: слева форма, справа картинка */
    .main-layout { display: flex; gap: 30px; align-items: flex-start; }
    .form-column { flex: 1; min-width: 0; }
    .image-column { flex: 0 0 300px; position: sticky; top: 20px; }
    
    @media (max-width: 768px) {
      .main-layout { flex-direction: column; }
      .image-column { flex: 1; position: static; width: 100%; }
      .image-column img { max-height: 200px; }
    }
    
    .form-group { margin-bottom: 20px; }
    label { display: block; font-weight: 600; margin-bottom: 6px; font-size: 14px; color: #1e293b; }
    select, input[type="checkbox"] { padding: 8px 12px; border-radius: 8px; border: 1px solid #d1d5db; font-size: 14px; width: 100%; background: white; }
    .row { display: flex; flex-wrap: wrap; gap: 16px; }
    .col { flex: 1 0 180px; }
    .checkbox-group { display: flex; align-items: center; gap: 8px; }
    .checkbox-group input { width: auto; }
    .price-block { background: #f8fafc; border-radius: 12px; padding: 16px; margin-top: 20px; border: 1px solid #e2e8f0; }
    .price-row { display: flex; justify-content: space-between; padding: 6px 0; border-bottom: 1px dashed #e2e8f0; }
    .price-row:last-child { border-bottom: none; }
    .total { font-size: 20px; font-weight: 700; color: #0f172a; }
    .highlight { background: #dbeafe; padding: 2px 8px; border-radius: 20px; }
    .hidden { display: none; }
    .btn { background: #1e293b; color: white; border: none; padding: 10px 20px; border-radius: 10px; font-weight: 600; cursor: pointer; }
    .btn:hover { background: #0f172a; }
    .mt-2 { margin-top: 12px; }
    .chip { background: #e2e8f0; padding: 4px 12px; border-radius: 30px; font-size: 13px; display: inline-block; }
    
    /* Стили для картинки */
    .image-container {
      background: #f8fafc;
      border-radius: 12px;
      border: 1px solid #e2e8f0;
      padding: 12px;
      text-align: center;
      min-height: 200px;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
    }
    .image-container img {
      max-width: 100%;
      max-height: 350px;
      border-radius: 8px;
      object-fit: contain;
    }
    .image-placeholder {
      color: #94a3b8;
      font-size: 14px;
      padding: 40px 20px;
    }
    .image-placeholder .icon { font-size: 48px; display: block; margin-bottom: 12px; }
  </style>
</head>
<body>
<div class="app" id="app">
  <h1>🚪 Конфигуратор дверей</h1>

  <!-- ОСНОВНОЙ МАКЕТ: форма слева, картинка справа -->
  <div class="main-layout">
    <!-- Левая колонка - форма -->
    <div class="form-column">
      <div class="form-group">
        <label>Тип конструкции</label>
        <select id="typeSelect"><option value="">— выберите —</option><option value="door">Дверь</option><option value="window">Окно</option></select>
      </div>

      <div class="form-group">
        <label>Система</label>
        <select id="systemSelect"><option value="">— выберите —</option><option value="AYPC.W72">AYPC.W72</option><option value="AYPC.W62">AYPC.W62</option><option value="AYPC.C48">AYPC.C48</option></select>
      </div>

      <div id="doorFields" class="hidden">
        <div class="form-group">
          <label>Количество створок</label>
          <select id="doortypeSelect"><option value="">— выберите —</option><option value="single-leaf">Одностворчатая</option><option value="double-leaf">Двухстворчатая</option></select>
        </div>
        <div class="form-group">
          <label>Конфигурация (глухие части)</label>
          <select id="blindSelect"><option value="">— выберите —</option><option value="none">Без глухих частей</option><option value="top">Глухарь сверху</option><option value="left-or-right">Глухарь сбоку</option><option value="left-and-right">Глухарь слева и справа</option></select>
        </div>
        <div class="form-group" id="thresholdGroup">
          <label>Высота порога</label>
          <select id="thresholdSelect"><option value="">— выберите —</option><option value="14">14 мм (один контур)</option><option value="22">22 мм (два контура)</option></select>
        </div>
      </div>

      <div class="form-group" id="sizeGroup">
        <label>Размер (ширина x высота)</label>
        <select id="sizeSelect"><option value="">— сначала выберите параметры выше —</option></select>
      </div>

      <div id="constructiveGroup" class="hidden">
        <div class="form-group checkbox-group">
          <input type="checkbox" id="impostSash" value="impost_sash">
          <label for="impostSash" style="margin:0; font-weight:400;">Импост в створке</label>
        </div>
        <div class="form-group checkbox-group hidden" id="impostBlindGroup">
          <input type="checkbox" id="impostBlind" value="impost_blind">
          <label for="impostBlind" style="margin:0; font-weight:400;">Импост в глухаре</label>
        </div>
      </div>

      <div class="form-group">
        <label>Ценовая опция</label>
        <select id="priceTypeSelect"><option value="wholesale">Оптовая</option><option value="base">Розничная</option></select>
      </div>

      <div class="form-group" id="lockGroup">
        <label>Тип замка</label>
        <select id="lockSelect"><option value="">— выберите —</option></select>
      </div>

      <div class="form-group" id="hingeGroup">
        <label>Тип петель</label>
        <select id="hingeSelect"><option value="">— выберите —</option></select>
      </div>

      <button class="btn" id="calcBtn">Рассчитать стоимость</button>

      <div id="result" class="price-block hidden">
        <h3>💰 Итоговая стоимость</h3>
        <div id="resultTotal" class="total" style="font-size:28px; margin: 12px 0;">0 ₽</div>
        <div id="resultBreakdown"></div>
      </div>
    </div>

    <!-- Правая колонка - картинка -->
    <div class="image-column">
      <div class="image-container" id="productImageContainer">
        <img id="productImage" src="" alt="Изделие" style="display: none;">
        <div class="image-placeholder" id="imagePlaceholder">
          <span class="icon">🖼️</span>
          <span>Выберите размер,<br>чтобы увидеть изображение</span>
        </div>
      </div>
    </div>
  </div>
</div>

<script>
const productsData = {
  "ID_1": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "900x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "900",
      "height": "2100",
      "area": "1,89",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "48469",
      "wholesale": "35722",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4881"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "8643"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "19368"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "13479"
            },
            "stublina_multi": {
              "label": "Stublina многозапорный",
              "price": "6060"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_1.png"
  },
  "ID_2": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "1000x2400"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "1000",
      "height": "2400",
      "area": "2,4",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "64040",
      "wholesale": "41274",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4920"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "15395"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_2.png"
  },
  "ID_3": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "1000x2600"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "1000",
      "height": "2600",
      "area": "2,6",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "76559",
      "wholesale": "48838",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4920"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "18855"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_3.png"
  },
  "ID_4": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "top",
      "size": "1000x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "top",
      "width": "1000",
      "height": "3000",
      "area": "3",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "82146",
      "wholesale": "53621",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4920"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "15395"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_4.png"
  },
  "ID_5": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "top",
      "size": "1000x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "top",
      "width": "1000",
      "height": "3000",
      "area": "3",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "94590",
      "wholesale": "58835",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4920"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "18855"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_5.png"
  },
  "ID_6": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "size": "1500x2400"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "width": "1500",
      "height": "2400",
      "area": "3,6",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "82881",
      "wholesale": "59828",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4920"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "4525"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "15395"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_6.png"
  },
  "ID_7": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "size": "1500x2600"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "width": "1500",
      "height": "2600",
      "area": "3,9",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "95523",
      "wholesale": "67515",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4920"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "4525"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "18855"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_7.png"
  },
  "ID_8": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "size": "2000x2400"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "width": "2000",
      "height": "2400",
      "area": "4,8",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "101148",
      "wholesale": "78382",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4920"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "9050"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "15395"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_8.png"
  },
  "ID_9": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "size": "2000x2600"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "width": "2000",
      "height": "2600",
      "area": "5,2",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "113913",
      "wholesale": "86192",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4920"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "9050"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "18855"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_9.png"
  },
  "ID_10": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "none",
      "size": "900x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "none",
      "width": "900",
      "height": "2100",
      "area": "1,89",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "69632",
      "wholesale": "37081",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4881"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "8643"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "19368"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "13479"
            },
            "stublina_multi": {
              "label": "Stublina многозапорный",
              "price": "6060"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_1.png"
  },
  "ID_11": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "none",
      "size": "1000x2400"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "none",
      "width": "1000",
      "height": "2400",
      "area": "2,4",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "69842",
      "wholesale": "43048",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4920"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "15395"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_2.png"
  },
  "ID_12": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "none",
      "size": "1000x2600"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "none",
      "width": "1000",
      "height": "2600",
      "area": "2,6",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "80462",
      "wholesale": "50334",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4920"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "18855"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_3.png"
  },
  "ID_13": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "top",
      "size": "1000x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "top",
      "width": "1000",
      "height": "3000",
      "area": "3",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "87951",
      "wholesale": "55397",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4920"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "15395"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_4.png"
  },
  "ID_14": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "top",
      "size": "1000x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "top",
      "width": "1000",
      "height": "3000",
      "area": "3",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "98493",
      "wholesale": "60330",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4920"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "18855"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_5.png"
  },
  "ID_15": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "size": "1500x2400"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "width": "1500",
      "height": "2400",
      "area": "3,6",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "88780",
      "wholesale": "61700",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4920"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "4525"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "15395"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_6.png"
  },
  "ID_16": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "size": "1500x2600"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "width": "1500",
      "height": "2600",
      "area": "3,9",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "99523",
      "wholesale": "69108",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4920"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "4525"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "18855"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_7.png"
  },
  "ID_17": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "size": "2000x2400"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "width": "2000",
      "height": "2400",
      "area": "4,8",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "107146",
      "wholesale": "80760",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4920"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "9050"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "15395"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_8.png"
  },
  "ID_18": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "size": "2000x2600"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "width": "2000",
      "height": "2600",
      "area": "5,2",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "118011",
      "wholesale": "88291",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "4920"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "9050"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "18855"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20single%20leaf%2014%20threshold/Screenshot_9.png"
  },
  "ID_19": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "900x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "900",
      "height": "2100",
      "area": "1,89",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "41879",
      "wholesale": "29351",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3797"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "8643"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "19368"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "13479"
            },
            "stublina_multi": {
              "label": "Stublina многозапорный",
              "price": "6060"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20single%20leaf%2020%20threshold/Screenshot_1.png"
  },
  "ID_20": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "900x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "900",
      "height": "2500",
      "area": "2,25",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "54344",
      "wholesale": "33666",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3797"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "15395"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20single%20leaf%2020%20threshold/Screenshot_2.png"
  },
  "ID_21": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "top",
      "size": "900x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "top",
      "width": "900",
      "height": "2500",
      "area": "2,25",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "55552",
      "wholesale": "36651",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3797"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "8643"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "19368"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "13479"
            },
            "stublina_multi": {
              "label": "Stublina многозапорный",
              "price": "6060"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20single%20leaf%2020%20threshold/Screenshot_3.png"
  },
  "ID_22": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "top",
      "size": "900x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "top",
      "width": "900",
      "height": "3000",
      "area": "2,7",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "68038",
      "wholesale": "40987",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3797"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "15395"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20single%20leaf%2020%20threshold/Screenshot_4.png"
  },
  "ID_23": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "size": "1500x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "width": "1500",
      "height": "2100",
      "area": "3,15",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "56075",
      "wholesale": "41683",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3817"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "3695"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "8643"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "19368"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "13479"
            },
            "stublina_multi": {
              "label": "Stublina многозапорный",
              "price": "6060"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20single%20leaf%2020%20threshold/Screenshot_5.png"
  },
  "ID_24": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "size": "1500x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "width": "1500",
      "height": "2500",
      "area": "3,75",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "68672",
      "wholesale": "48116",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3817"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "3695"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "15395"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20single%20leaf%2020%20threshold/Screenshot_6.png"
  },
  "ID_25": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "size": "2000x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "width": "2000",
      "height": "2100",
      "area": "4,2",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "69645",
      "wholesale": "53961",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3817"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "7390"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "8643"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "19368"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "13479"
            },
            "stublina_multi": {
              "label": "Stublina многозапорный",
              "price": "6060"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20single%20leaf%2020%20threshold/Screenshot_7.png"
  },
  "ID_26": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "size": "2000x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "width": "2000",
      "height": "2500",
      "area": "5",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "82373",
      "wholesale": "62512",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3817"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "7390"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "15395"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20single%20leaf%2020%20threshold/Screenshot_8.png"
  },
  "ID_27": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "none",
      "size": "900x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "none",
      "width": "900",
      "height": "2100",
      "area": "1,89",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "54407",
      "wholesale": "29344",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3797"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "8643"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "19368"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "13479"
            },
            "stublina_multi": {
              "label": "Stublina многозапорный",
              "price": "6060"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20single%20leaf%2020%20threshold/Screenshot_1.png"
  },
  "ID_28": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "none",
      "size": "900x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "none",
      "width": "900",
      "height": "2500",
      "area": "2,25",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "54527",
      "wholesale": "33659",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3797"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "15395"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20single%20leaf%2020%20threshold/Screenshot_2.png"
  },
  "ID_29": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "top",
      "size": "900x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "top",
      "width": "900",
      "height": "2500",
      "area": "2,25",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "68080",
      "wholesale": "36644",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3797"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "8643"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "19368"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "13479"
            },
            "stublina_multi": {
              "label": "Stublina многозапорный",
              "price": "6060"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20single%20leaf%2020%20threshold/Screenshot_3.png"
  },
  "ID_30": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "top",
      "size": "900x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "top",
      "width": "900",
      "height": "3000",
      "area": "2,7",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "68221",
      "wholesale": "40979",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3797"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "15395"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20single%20leaf%2020%20threshold/Screenshot_4.png"
  },
  "ID_31": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "size": "1500x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "width": "1500",
      "height": "2100",
      "area": "3,15",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "68597",
      "wholesale": "41670",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3817"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "3695"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "8643"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "19368"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "13479"
            },
            "stublina_multi": {
              "label": "Stublina многозапорный",
              "price": "6060"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20single%20leaf%2020%20threshold/Screenshot_5.png"
  },
  "ID_32": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "size": "1500x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "width": "1500",
      "height": "2500",
      "area": "3,75",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "68849",
      "wholesale": "48102",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3817"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "3695"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "15395"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20single%20leaf%2020%20threshold/Screenshot_6.png"
  },
  "ID_33": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "size": "2000x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "width": "2000",
      "height": "2100",
      "area": "4,2",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "82166",
      "wholesale": "53947",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3817"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "7390"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "8643"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "19368"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "13479"
            },
            "stublina_multi": {
              "label": "Stublina многозапорный",
              "price": "6060"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20single%20leaf%2020%20threshold/Screenshot_7.png"
  },
  "ID_34": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "size": "2000x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "single-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "width": "2000",
      "height": "2500",
      "area": "5",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "82549",
      "wholesale": "62498",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3817"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "7390"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11524"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "25823"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_single": {
              "label": "FUHR (одностворчатая)",
              "price": "15395"
            },
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1464"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20single%20leaf%2020%20threshold/Screenshot_8.png"
  },
  "ID_35": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "900x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "900",
      "height": "2100",
      "area": "1,89",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "23080",
      "wholesale": "17767",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "2331"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "5780"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1676"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20single%20leaf/Screenshot_1.png"
  },
  "ID_36": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "900x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "900",
      "height": "2500",
      "area": "2,25",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "30278",
      "wholesale": "20305",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "2331"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "7707"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1676"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20single%20leaf/Screenshot_2.png"
  },
  "ID_37": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "top",
      "size": "900x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "top",
      "width": "900",
      "height": "2500",
      "area": "2,25",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "32142",
      "wholesale": "22672",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "2331"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "5780"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1676"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20single%20leaf/Screenshot_3.png"
  },
  "ID_38": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "top",
      "size": "900x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "top",
      "width": "900",
      "height": "3000",
      "area": "2,7",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "39356",
      "wholesale": "25227",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "2331"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "7707"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1676"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20single%20leaf/Screenshot_4.png"
  },
  "ID_39": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "size": "1500x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "width": "1500",
      "height": "2100",
      "area": "3,15",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "32429",
      "wholesale": "25757",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "2347"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "1943"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "5780"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1676"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20single%20leaf/Screenshot_5.png"
  },
  "ID_40": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "size": "1500x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "width": "1500",
      "height": "2500",
      "area": "3,75",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "39723",
      "wholesale": "29750",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "2347"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "1943"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "7707"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1676"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20single%20leaf/Screenshot_6.png"
  },
  "ID_41": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "size": "2000x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "width": "2000",
      "height": "2100",
      "area": "4,2",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "41744",
      "wholesale": "33712",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "2347"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "3886"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "5780"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1676"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20single%20leaf/Screenshot_7.png"
  },
  "ID_42": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "size": "2000x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "single-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "width": "2000",
      "height": "2500",
      "area": "5",
      "wholesale_quantity": "Цена за шт при заказе 6 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "49134",
      "wholesale": "39161",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "2347"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "3886"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "7707"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single": {
              "label": "Stublina однозапорный",
              "price": "1676"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20single%20leaf/Screenshot_8.png"
  },
  "ID_43": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "1500x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "1500",
      "height": "2100",
      "area": "3,15",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "83945",
      "wholesale": "59249",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "30655"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_1.png"
  },
  "ID_44": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "1500x2400"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "1500",
      "height": "2400",
      "area": "3,6",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "84219",
      "wholesale": "63730",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32571"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_2.png"
  },
  "ID_45": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "1500x2600"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "1500",
      "height": "2600",
      "area": "3,9",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "118977",
      "wholesale": "82381",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "36155"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_3.png"
  },
  "ID_46": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "1800x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "1800",
      "height": "2100",
      "area": "3,78",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "84127",
      "wholesale": "60304",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "10297"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "30655"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_4.png"
  },
  "ID_47": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "1800x2400"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "1800",
      "height": "2400",
      "area": "4,32",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "99661",
      "wholesale": "71275",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "10297"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32571"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_5.png"
  },
  "ID_48": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "1800x2600"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "1800",
      "height": "2600",
      "area": "4,68",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "119147",
      "wholesale": "93767",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "10297"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "36155"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_6.png"
  },
  "ID_49": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "size": "2000x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "width": "2000",
      "height": "2100",
      "area": "4,2",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "102627",
      "wholesale": "77278",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "5941"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "30655"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_7.png"
  },
  "ID_50": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "size": "2000x2400"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "width": "2000",
      "height": "2400",
      "area": "4,8",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "103060",
      "wholesale": "82284",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "5941"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32571"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_8.png"
  },
  "ID_51": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "size": "2000x2600"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "width": "2000",
      "height": "2600",
      "area": "5,2",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "137940",
      "wholesale": "101058",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "5941"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "36155"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_9.png"
  },
  "ID_52": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "size": "2500x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "width": "2500",
      "height": "2100",
      "area": "5,25",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "120735",
      "wholesale": "91751",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "11882"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "30655"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_10.png"
  },
  "ID_53": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "size": "2500x2400"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "width": "2500",
      "height": "2400",
      "area": "6",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "121327",
      "wholesale": "100838",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "11882"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32571"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_11.png"
  },
  "ID_54": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "size": "2500x2600"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "width": "2500",
      "height": "2600",
      "area": "6,5",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "156331",
      "wholesale": "119735",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "11882"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "36155"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_12.png"
  },
  "ID_55": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "size": "1500x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "width": "1500",
      "height": "3000",
      "area": "4,5",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "102474",
      "wholesale": "76616",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "30655"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_13.png"
  },
  "ID_56": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "size": "1500x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "width": "1500",
      "height": "3000",
      "area": "4,5",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "102631",
      "wholesale": "77568",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32571"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_14.png"
  },
  "ID_57": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "size": "1500x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "width": "1500",
      "height": "3000",
      "area": "4,5",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "137311",
      "wholesale": "96142",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "36155"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_15.png"
  },
  "ID_58": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "size": "1500x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "width": "1500",
      "height": "2100",
      "area": "3,15",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "105223",
      "wholesale": "61778",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32919"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_1.png"
  },
  "ID_59": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "size": "1500x2400"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "width": "1500",
      "height": "2400",
      "area": "3,6",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "105497",
      "wholesale": "66260",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "34835"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_2.png"
  },
  "ID_60": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "size": "1500x2600"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "width": "1500",
      "height": "2600",
      "area": "3,9",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "143063",
      "wholesale": "84139",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "38419"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_3.png"
  },
  "ID_61": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "size": "1800x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "width": "1800",
      "height": "2100",
      "area": "3,78",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "105448",
      "wholesale": "62708",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "10297"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32919"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_4.png"
  },
  "ID_62": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "size": "1800x2400"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "width": "1800",
      "height": "2400",
      "area": "4,32",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "120982",
      "wholesale": "78801",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "10297"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "34835"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_5.png"
  },
  "ID_63": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "size": "1800x2600"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "width": "1800",
      "height": "2600",
      "area": "4,68",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "144561",
      "wholesale": "95614",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "10297"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "38419"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_6.png"
  },
  "ID_64": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "size": "2000x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "width": "2000",
      "height": "2100",
      "area": "4,2",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "124002",
      "wholesale": "79905",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "5941"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32919"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_7.png"
  },
  "ID_65": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "size": "2000x2400"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "width": "2000",
      "height": "2400",
      "area": "4,8",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "124435",
      "wholesale": "84911",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "5941"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "34835"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_8.png"
  },
  "ID_66": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "size": "2000x2600"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "width": "2000",
      "height": "2600",
      "area": "5,2",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "163397",
      "wholesale": "103280",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "5941"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "38419"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_9.png"
  },
  "ID_67": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "size": "2500x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "width": "2500",
      "height": "2100",
      "area": "5,25",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "142208",
      "wholesale": "94476",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "11882"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32919"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_10.png"
  },
  "ID_68": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "size": "2500x2400"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "width": "2500",
      "height": "2400",
      "area": "6",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "142800",
      "wholesale": "103563",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "11882"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "34835"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_11.png"
  },
  "ID_69": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "size": "2500x2600"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "width": "2500",
      "height": "2600",
      "area": "6,5",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "181885",
      "wholesale": "122054",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "11882"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "38419"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_12.png"
  },
  "ID_70": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "top",
      "size": "1500x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "top",
      "width": "1500",
      "height": "3000",
      "area": "4,5",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "123751",
      "wholesale": "79145",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32919"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_13.png"
  },
  "ID_71": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "top",
      "size": "1500x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "top",
      "width": "1500",
      "height": "3000",
      "area": "4,5",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "123909",
      "wholesale": "80098",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "34835"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_14.png"
  },
  "ID_72": {
    "key": {
      "type": "door",
      "system": "AYPC.W72",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "top",
      "size": "1500x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W72",
      "subsystem": "HI+, anti bi-metal",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "top",
      "width": "1500",
      "height": "3000",
      "area": "4,5",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "162670",
      "wholesale": "98266",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8133"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1346"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "38419"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W72%20double%20leaf%2020%20threshold/Screenshot_15.png"
  },
  "ID_73": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "1500x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "1500",
      "height": "2100",
      "area": "3,15",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "70654",
      "wholesale": "49237",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "6348"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "30655"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_1.png"
  },
  "ID_74": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "1500x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "1500",
      "height": "2500",
      "area": "3,75",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "82363",
      "wholesale": "55749",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "6348"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "36155"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_2.png"
  },
  "ID_75": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "1800x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "1800",
      "height": "2100",
      "area": "3,78",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "70838",
      "wholesale": "49736",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8061"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "30655"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_3.png"
  },
  "ID_76": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "1800x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "1800",
      "height": "2500",
      "area": "4,5",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "82546",
      "wholesale": "62460",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8061"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "36155"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_4.png"
  },
  "ID_77": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "size": "1500x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "width": "1500",
      "height": "2500",
      "area": "3,75",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "84538",
      "wholesale": "59521",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "6348"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "30655"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_5.png"
  },
  "ID_78": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "size": "1500x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "width": "1500",
      "height": "3000",
      "area": "4,5",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "96267",
      "wholesale": "66053",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "6348"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "36155"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_6.png"
  },
  "ID_79": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "size": "1800x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "width": "1800",
      "height": "2500",
      "area": "4,5",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "84824",
      "wholesale": "62896",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8061"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "30655"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_7.png"
  },
  "ID_80": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "size": "1800x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "width": "1800",
      "height": "3000",
      "area": "5,4",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "96553",
      "wholesale": "75641",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8061"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "36155"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_8.png"
  },
  "ID_81": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "size": "2000x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "width": "2000",
      "height": "2100",
      "area": "4,2",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "84796",
      "wholesale": "62760",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "6348"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "4546"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "30655"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_9.png"
  },
  "ID_82": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "size": "2000x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "width": "2000",
      "height": "2500",
      "area": "5",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "96637",
      "wholesale": "69736",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "6348"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "4546"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "36155"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_10.png"
  },
  "ID_83": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "size": "2300x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "width": "2300",
      "height": "2100",
      "area": "4,83",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "84980",
      "wholesale": "64313",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8061"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "4546"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "30655"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_11.png"
  },
  "ID_84": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "size": "2300x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "width": "2300",
      "height": "2500",
      "area": "5,75",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "96820",
      "wholesale": "77360",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8061"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "4546"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "36155"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_12.png"
  },
  "ID_85": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "size": "2500x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "width": "2500",
      "height": "2100",
      "area": "5,25",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "98366",
      "wholesale": "73636",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "6348"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "9092"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "30655"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_13.png"
  },
  "ID_86": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "size": "2500x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "width": "2500",
      "height": "2500",
      "area": "6,25",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "110338",
      "wholesale": "83724",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "6348"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "9092"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "36155"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_14.png"
  },
  "ID_87": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "size": "2800x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "width": "2800",
      "height": "2100",
      "area": "5,88",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "98549",
      "wholesale": "74291",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8061"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "9092"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "30655"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_15.png"
  },
  "ID_88": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "size": "2800x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "width": "2800",
      "height": "2500",
      "area": "7",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "110521",
      "wholesale": "91252",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8061"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "9092"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "36155"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_16.png"
  },
  "ID_89": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "size": "1500x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "width": "1500",
      "height": "2100",
      "area": "3,15",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "83147",
      "wholesale": "49213",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "6348"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32919"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_1.png"
  },
  "ID_90": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "size": "1500x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "width": "1500",
      "height": "2500",
      "area": "3,75",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "94856",
      "wholesale": "55726",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "6348"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "38419"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_2.png"
  },
  "ID_91": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "size": "1800x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "width": "1800",
      "height": "2100",
      "area": "3,78",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "83317",
      "wholesale": "49718",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8061"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32919"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_3.png"
  },
  "ID_92": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "size": "1800x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "none",
      "width": "1800",
      "height": "2500",
      "area": "4,5",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "95026",
      "wholesale": "62442",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8061"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "38419"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_4.png"
  },
  "ID_93": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "top",
      "size": "1500x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "top",
      "width": "1500",
      "height": "2500",
      "area": "3,75",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "97030",
      "wholesale": "59497",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "6348"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32919"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_5.png"
  },
  "ID_94": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "top",
      "size": "1500x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "top",
      "width": "1500",
      "height": "3000",
      "area": "4,5",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "108760",
      "wholesale": "66030",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "6348"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "38419"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_6.png"
  },
  "ID_95": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "top",
      "size": "1800x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "top",
      "width": "1800",
      "height": "2500",
      "area": "4,5",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "97303",
      "wholesale": "62878",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8061"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32919"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_7.png"
  },
  "ID_96": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "top",
      "size": "1800x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "top",
      "width": "1800",
      "height": "3000",
      "area": "5,4",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "109033",
      "wholesale": "75623",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8061"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "38419"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_8.png"
  },
  "ID_97": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "size": "2000x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "width": "2000",
      "height": "2100",
      "area": "4,2",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "97289",
      "wholesale": "62736",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "6348"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "4546"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32919"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_9.png"
  },
  "ID_98": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "size": "2000x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "width": "2000",
      "height": "2500",
      "area": "5",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "109129",
      "wholesale": "69713",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "6348"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "4546"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "38419"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_10.png"
  },
  "ID_99": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "size": "2300x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "width": "2300",
      "height": "2100",
      "area": "4,83",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "97459",
      "wholesale": "64295",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8061"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "4546"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32919"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_11.png"
  },
  "ID_100": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "size": "2300x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-or-right",
      "width": "2300",
      "height": "2500",
      "area": "5,75",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "109300",
      "wholesale": "77342",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8061"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "4546"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "38419"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_12.png"
  },
  "ID_101": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "size": "2500x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "width": "2500",
      "height": "2100",
      "area": "5,25",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "110859",
      "wholesale": "73612",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "6348"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "9092"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32919"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_13.png"
  },
  "ID_102": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "size": "2500x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "width": "2500",
      "height": "2500",
      "area": "6,25",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "122830",
      "wholesale": "83700",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "6348"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "9092"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "38419"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_14.png"
  },
  "ID_103": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "size": "2800x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "width": "2800",
      "height": "2100",
      "area": "5,88",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "111029",
      "wholesale": "74273",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8061"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "9092"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "17284"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "38735"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "32919"
            },
            "stublina_multi_visible": {
              "label": "Stublina многозапорный (видимый штифт)",
              "price": "8201"
            },
            "stublina_multi_hidden": {
              "label": "Stublina многозапорный (скрытый штифт)",
              "price": "7844"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_15.png"
  },
  "ID_104": {
    "key": {
      "type": "door",
      "system": "AYPC.W62",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "size": "2800x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.W62",
      "subsystem": "st изолятор",
      "doortype": "double-leaf",
      "threshold": "22",
      "blind": "left-and-right",
      "width": "2800",
      "height": "2500",
      "area": "7",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "123000",
      "wholesale": "91234",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "8061"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "9092"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1244"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "23046"
            },
            "roller": {
              "label": "Роликовые петли",
              "price": "51645"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "fuhr_double": {
              "label": "FUHR (двухстворчатая)",
              "price": "38419"
            },
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/W62%20double%20leaf%2020%20threshold/Screenshot_16.png"
  },
  "ID_105": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "1500x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "1500",
      "height": "2100",
      "area": "3,15",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "41732",
      "wholesale": "30577",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3873"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11560"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20double%20leaf/Screenshot_1.png"
  },
  "ID_106": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "1500x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "1500",
      "height": "2500",
      "area": "3,75",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "47825",
      "wholesale": "34417",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3873"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "15414"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20double%20leaf/Screenshot_2.png"
  },
  "ID_107": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "1800x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "1800",
      "height": "2100",
      "area": "3,78",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "41844",
      "wholesale": "30959",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "5222"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11560"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20double%20leaf/Screenshot_3.png"
  },
  "ID_108": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "size": "1800x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "none",
      "width": "1800",
      "height": "2500",
      "area": "4,5",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "47937",
      "wholesale": "38385",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "5222"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "15414"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20double%20leaf/Screenshot_4.png"
  },
  "ID_109": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "size": "1500x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "width": "1500",
      "height": "2500",
      "area": "3,75",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "50945",
      "wholesale": "37345",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3873"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11560"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20double%20leaf/Screenshot_5.png"
  },
  "ID_110": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "size": "1500x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "width": "1500",
      "height": "3000",
      "area": "4,5",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "57054",
      "wholesale": "41202",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3873"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "15414"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20double%20leaf/Screenshot_6.png"
  },
  "ID_111": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "size": "1800x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "width": "1800",
      "height": "2500",
      "area": "4,5",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "51121",
      "wholesale": "39504",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "5222"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11560"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20double%20leaf/Screenshot_7.png"
  },
  "ID_112": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "size": "1800x3000"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "top",
      "width": "1800",
      "height": "3000",
      "area": "5,4",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "57230",
      "wholesale": "46946",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "5222"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "15414"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20double%20leaf/Screenshot_8.png"
  },
  "ID_113": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "size": "2000x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "width": "2000",
      "height": "2100",
      "area": "4,2",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "51047",
      "wholesale": "39342",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3873"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "2601"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11560"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20double%20leaf/Screenshot_9.png"
  },
  "ID_114": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "size": "2000x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "width": "2000",
      "height": "2500",
      "area": "5",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "57236",
      "wholesale": "43828",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3873"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "2601"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "15414"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20double%20leaf/Screenshot_10.png"
  },
  "ID_115": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "size": "2300x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "width": "2300",
      "height": "2100",
      "area": "4,83",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "51158",
      "wholesale": "40083",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "5222"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "2601"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11560"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20double%20leaf/Screenshot_11.png"
  },
  "ID_116": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "size": "2300x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-or-right",
      "width": "2300",
      "height": "2500",
      "area": "5,75",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "57348",
      "wholesale": "47795",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "5222"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "2601"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "15414"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20double%20leaf/Screenshot_12.png"
  },
  "ID_117": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "size": "2500x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "width": "2500",
      "height": "2100",
      "area": "5,25",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "60361",
      "wholesale": "46762",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3873"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "5202"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11560"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20double%20leaf/Screenshot_13.png"
  },
  "ID_118": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "size": "2500x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "width": "2500",
      "height": "2500",
      "area": "6,25",
      "wholesale_quantity": "Цена за шт при заказе 4 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "66647",
      "wholesale": "53539",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "3873"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "5202"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "15414"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20double%20leaf/Screenshot_14.png"
  },
  "ID_119": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "size": "2800x2100"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "width": "2800",
      "height": "2100",
      "area": "5,88",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "3"
    },
    "price": {
      "base": "60473",
      "wholesale": "46870",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "5222"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "5202"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "11560"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20double%20leaf/Screenshot_15.png"
  },
  "ID_120": {
    "key": {
      "type": "door",
      "system": "AYPC.C48",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "size": "2800x2500"
    },
    "info": {
      "type": "door",
      "system": "AYPC.C48",
      "subsystem": "Без терморазрыва",
      "doortype": "double-leaf",
      "threshold": "14",
      "blind": "left-and-right",
      "width": "2800",
      "height": "2500",
      "area": "7",
      "wholesale_quantity": "Цена за шт при заказе 3 шт",
      "hinge_quantity": "4"
    },
    "price": {
      "base": "66758",
      "wholesale": "57206",
      "constructive": {
        "impost_sash": {
          "type": "checkbox",
          "label": "Импост в створке",
          "price": "5222"
        },
        "impost_blind": {
          "type": "checkbox",
          "label": "Импост в глухаре",
          "price": "5202"
        }
      }
    },
    "furniture": {
      "fixed": {
        "cylinder": {
          "label": "Цилиндровый механизм",
          "price": "1033"
        },
        "door_handle": {
          "label": "Нажимной гарнитур",
          "price": "1449"
        }
      },
      "selectable": {
        "hinge": {
          "type": "select",
          "label": "Тип петель",
          "variants": {
            "overhead": {
              "label": "Накладные петли",
              "price": "15414"
            }
          }
        },
        "lock": {
          "type": "select",
          "label": "Тип замка",
          "variants": {
            "stublina_single_double_hidden": {
              "label": "Stublina однозапорный (двухстворчатая, скрытый штифт)",
              "price": "3604"
            },
            "stublina_single_double_visible": {
              "label": "Stublina однозапорный (двухстворчатая, видимый штифт)",
              "price": "3247"
            }
          }
        }
      }
    },
    "image": "https://raw.githubusercontent.com/anatoliykutcenko/img/refs/heads/main/C48%20double%20leaf/Screenshot_16.png"
  }
};



// ===== DOM ЭЛЕМЕНТЫ =====
const typeEl = document.getElementById('typeSelect');
const systemEl = document.getElementById('systemSelect');
const doortypeEl = document.getElementById('doortypeSelect');
const blindEl = document.getElementById('blindSelect');
const thresholdEl = document.getElementById('thresholdSelect');
const sizeEl = document.getElementById('sizeSelect');
const constructiveGroup = document.getElementById('constructiveGroup');
const impostSashChk = document.getElementById('impostSash');
const impostBlindChk = document.getElementById('impostBlind');
const impostBlindGroup = document.getElementById('impostBlindGroup');
const priceTypeEl = document.getElementById('priceTypeSelect');
const lockEl = document.getElementById('lockSelect');
const hingeEl = document.getElementById('hingeSelect');
const resultDiv = document.getElementById('result');
const resultTotal = document.getElementById('resultTotal');
const resultBreakdown = document.getElementById('resultBreakdown');

const doorFields = document.getElementById('doorFields');
const thresholdGroup = document.getElementById('thresholdGroup');

// ===== ВСПОМОГАТЕЛЬНЫЕ ФУНКЦИИ =====
function getIdsByKey(filter) {
  return Object.keys(productsData).filter(id => {
    const k = productsData[id].key;
    for (let key in filter) {
      if (filter[key] !== undefined && k[key] != filter[key]) return false;
    }
    return true;
  });
}

function getSizeOptions(ids) {
  const sizes = new Set();
  ids.forEach(id => {
    const info = productsData[id].info;
    if (info && info.width && info.height) {
      sizes.add(`${info.width}x${info.height}`);
    }
  });
  return [...sizes].sort();
}

function getProductBySize(size, ids) {
  const [w, h] = size.split('x');
  return ids.find(id => productsData[id].info.width === w && productsData[id].info.height === h);
}

function getSelectableVariants(productId, category) {
  const sel = productsData[productId]?.furniture?.selectable?.[category];
  if (!sel || sel.type !== 'select') return {};
  return sel.variants || {};
}

function getConstructiveOptions(productId) {
  return productsData[productId]?.price?.constructive || {};
}

// ===== ФУНКЦИЯ ПОКАЗА КАРТИНКИ =====
function updateImage(productId) {
  const imgContainer = document.getElementById('productImageContainer');
  const img = document.getElementById('productImage');
  const placeholder = document.getElementById('imagePlaceholder');
  
  if (productId && productsData[productId] && productsData[productId].image) {
    const imageUrl = productsData[productId].image;
    img.src = imageUrl;
    img.style.display = 'block';
    placeholder.style.display = 'none';
    console.log('🖼️ Показываем картинку:', imageUrl);
  } else {
    img.style.display = 'none';
    placeholder.style.display = 'block';
    console.log('🖼️ Картинки нет для этого товара');
  }
}

// ===== ОБНОВЛЕНИЕ ПОЛЕЙ =====
function updateDoorFields() {
  const type = typeEl.value;
  doorFields.classList.toggle('hidden', type !== 'door');
  if (type !== 'door') {
    doortypeEl.value = '';
    blindEl.value = '';
    thresholdEl.value = '';
  }
  updateThresholdVisibility();
  updateSizeOptions();
}

function updateThresholdVisibility() {
  const system = systemEl.value;
  const type = typeEl.value;
  if (type === 'door' && (system === 'AYPC.W72' || system === 'AYPC.W62')) {
    thresholdGroup.classList.remove('hidden');
  } else if (type === 'door' && system === 'AYPC.C48') {
    thresholdGroup.classList.add('hidden');
    thresholdEl.value = '14';
  } else {
    thresholdGroup.classList.add('hidden');
  }
}

function updateSizeOptions() {
  const filter = {
    type: typeEl.value || undefined,
    system: systemEl.value || undefined,
    doortype: doortypeEl.value || undefined,
    blind: blindEl.value || undefined,
    threshold: thresholdEl.value || undefined
  };
  Object.keys(filter).forEach(k => filter[k] === undefined && delete filter[k]);

  const ids = getIdsByKey(filter);
  const sizes = getSizeOptions(ids);
  sizeEl.innerHTML = '<option value="">— выберите размер —</option>';
  sizes.forEach(s => {
    const opt = document.createElement('option');
    opt.value = s;
    opt.textContent = s;
    sizeEl.appendChild(opt);
  });

  if (sizes.length === 1) {
    sizeEl.value = sizes[0];
  }
  updateConstructiveAndFurniture();
}

function updateConstructiveAndFurniture() {
  const size = sizeEl.value;
  if (!size) {
    updateImage(null);
    constructiveGroup.classList.add('hidden');
    lockEl.innerHTML = '<option value="">— сначала выберите размер —</option>';
    hingeEl.innerHTML = '<option value="">— сначала выберите размер —</option>';
    return;
  }

  const ids = getIdsByKey({
    type: typeEl.value || undefined,
    system: systemEl.value || undefined,
    doortype: doortypeEl.value || undefined,
    blind: blindEl.value || undefined,
    threshold: thresholdEl.value || undefined
  });
  
  const productId = getProductBySize(size, ids);
  
  // ПОКАЗЫВАЕМ КАРТИНКУ
  updateImage(productId);
  
  if (!productId) {
    constructiveGroup.classList.add('hidden');
    lockEl.innerHTML = '<option value="">— товар не найден —</option>';
    hingeEl.innerHTML = '<option value="">— товар не найден —</option>';
    return;
  }

  const product = productsData[productId];

  // Конструктивные опции
  const constr = product.price?.constructive || {};
  const hasSash = !!constr.impost_sash;
  const hasBlind = !!constr.impost_blind;
  constructiveGroup.classList.remove('hidden');
  impostSashChk.checked = false;
  impostSashChk.parentElement.classList.toggle('hidden', !hasSash);
  impostBlindChk.checked = false;
  impostBlindGroup.classList.toggle('hidden', !hasBlind);

  // Замки
  const locks = getSelectableVariants(productId, 'lock');
  lockEl.innerHTML = '<option value="">— выберите —</option>';
  Object.keys(locks).forEach(k => {
    const opt = document.createElement('option');
    opt.value = k;
    opt.textContent = locks[k].label + ' (+' + locks[k].price + ' ₽)';
    lockEl.appendChild(opt);
  });

  // Петли
  const hinges = getSelectableVariants(productId, 'hinge');
  hingeEl.innerHTML = '<option value="">— выберите —</option>';
  Object.keys(hinges).forEach(k => {
    const opt = document.createElement('option');
    opt.value = k;
    opt.textContent = hinges[k].label + ' (+' + hinges[k].price + ' ₽)';
    hingeEl.appendChild(opt);
  });
}

// ===== РАСЧЕТ =====
function calculate() {
  const type = typeEl.value;
  const system = systemEl.value;
  const doortype = doortypeEl.value;
  const blind = blindEl.value;
  const threshold = thresholdEl.value;
  const size = sizeEl.value;
  const priceType = priceTypeEl.value;
  const lockKey = lockEl.value;
  const hingeKey = hingeEl.value;
  const impostSash = impostSashChk.checked;
  const impostBlind = impostBlindChk.checked;

  if (!type || !system || !size || !lockKey || !hingeKey) {
    alert('Заполните все обязательные поля (тип, система, размер, замок, петли)');
    return;
  }

  const ids = getIdsByKey({ type, system, doortype, blind, threshold });
  const productId = getProductBySize(size, ids);
  if (!productId) {
    alert('Не найден товар для выбранных параметров');
    return;
  }

  const product = productsData[productId];
  const basePrice = parseInt(product.price[priceType]) || 0;
  const constr = product.price.constructive || {};
  let constructiveSum = 0;
  let constructiveDetails = [];

  if (impostSash && constr.impost_sash) {
    const p = parseInt(constr.impost_sash.price) || 0;
    constructiveSum += p;
    constructiveDetails.push({ label: constr.impost_sash.label, price: p });
  }
  if (impostBlind && constr.impost_blind) {
    const p = parseInt(constr.impost_blind.price) || 0;
    constructiveSum += p;
    constructiveDetails.push({ label: constr.impost_blind.label, price: p });
  }

  const fixed = product.furniture.fixed || {};
  let fixedSum = 0;
  let fixedDetails = [];
  Object.values(fixed).forEach(item => {
    const p = parseInt(item.price) || 0;
    fixedSum += p;
    fixedDetails.push({ label: item.label, price: p });
  });

  const lockVar = product.furniture.selectable?.lock?.variants?.[lockKey];
  const hingeVar = product.furniture.selectable?.hinge?.variants?.[hingeKey];
  let selectableSum = 0;
  let selectableDetails = [];
  if (lockVar) {
    const p = parseInt(lockVar.price) || 0;
    selectableSum += p;
    selectableDetails.push({ label: lockVar.label, price: p });
  }
  if (hingeVar) {
    const p = parseInt(hingeVar.price) || 0;
    selectableSum += p;
    selectableDetails.push({ label: hingeVar.label, price: p });
  }

  const total = basePrice + constructiveSum + fixedSum + selectableSum;

  resultDiv.classList.remove('hidden');
  resultTotal.textContent = total.toLocaleString() + ' ₽';

  let html = `<div class="price-row"><span>Базовая цена (${priceType === 'wholesale' ? 'опт' : 'розница'})</span><span>${basePrice.toLocaleString()} ₽</span></div>`;
  constructiveDetails.forEach(d => {
    html += `<div class="price-row"><span>➕ ${d.label}</span><span>+${d.price.toLocaleString()} ₽</span></div>`;
  });
  fixedDetails.forEach(d => {
    html += `<div class="price-row"><span>🔒 ${d.label}</span><span>+${d.price.toLocaleString()} ₽</span></div>`;
  });
  selectableDetails.forEach(d => {
    html += `<div class="price-row"><span>🔧 ${d.label}</span><span>+${d.price.toLocaleString()} ₽</span></div>`;
  });
  html += `<div class="price-row total" style="border-top:2px solid #1e293b; margin-top:8px; padding-top:10px;"><span>Итого</span><span>${total.toLocaleString()} ₽</span></div>`;
  resultBreakdown.innerHTML = html;
}

// ===== СОБЫТИЯ =====
typeEl.addEventListener('change', updateDoorFields);
systemEl.addEventListener('change', () => { updateThresholdVisibility(); updateSizeOptions(); });
doortypeEl.addEventListener('change', updateSizeOptions);
blindEl.addEventListener('change', updateSizeOptions);
thresholdEl.addEventListener('change', updateSizeOptions);
sizeEl.addEventListener('change', updateConstructiveAndFurniture);
document.getElementById('calcBtn').addEventListener('click', calculate);

// Инициализация
updateDoorFields();
updateSizeOptions();
</script>
</body>
</html>