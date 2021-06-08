<template>
  <div class="container">
    <div class="panel flex overflow-auto ml-4">
      <div
        class="panel-elm panel-1 flex items-center justify-center flex-shrink-0"
        :class="{ selected: selected == 0 }"
        @click="change(0)"
      >
        <p class="text-center">Arbeitnehmer</p>
      </div>
      <div
        class="panel-elm flex items-center justify-center flex-shrink-0"
        :class="{ selected: selected == 1 }"
        @click="change(1)"
      >
        <p class="text-center">Arbeitgeber</p>
      </div>
      <div
        class="
          panel-elm
          flex
          items-center
          justify-center
          flex-shrink-0
          panel-3
          mr-4
        "
        :class="{ selected: selected == 2 }"
        @click="change(2)"
      >
        <p class="text-center">Temporärbüro</p>
      </div>
    </div>
    <Panelelm
      v-if="selected == 0"
      :h2="'Drei einfache Schritte zu deinem neuen Job'"
      :p1="'Erstellen dein Lebenslauf'"
      :p2="'Erstellen dein Lebenslauf'"
      :p3="'Mit nur einem Klick bewerben'"
      :img1="'undraw_Profile_data_re_v81r'"
      :img2="'undraw_task_31wc'"
      :img3="'undraw_personal_file_222m'"
    />
    <Panelelm
      v-if="selected == 1"
      :h2="'Drei einfache Schritte zu deinem neuen Mitarbeiter'"
      :p1="'Erstellen dein Unternehmensprofil'"
      :p2="'Erstellen ein Jobinserat'"
      :p3="'Wähle deinen neuen Mitarbeiter aus'"
      :img1="'undraw_Profile_data_re_v81r'"
      :img2="'undraw_about_me_wa29'"
      :img3="'undraw_swipe_profiles1_i6mr'"
    />
    <Panelelm
      v-if="selected == 2"
      :h2="'Drei einfache Schritte zur Vermittlung neuer Mitarbeiter'"
      :p1="'Erstellen dein Unternehmensprofil'"
      :p2="'Erhalte Vermittlungs- angebot von Arbeitgeber'"
      :p3="'Vermittlung nach Provision oder Stundenlohn'"
      :img1="'undraw_Profile_data_re_v81r'"
      :img2="'undraw_job_offers_kw5d'"
      :img3="'undraw_business_deal_cpi9'"
    />
  </div>
</template>

<script>
export default {
  data() {
    return {
      selected: 0,
    }
  },
  methods: {
    change(index) {
      this.selected = index
    },
  },
}
</script>

<style>
.panel {
  width: 481px;
  height: 40px;
  max-width: calc(100% - 1rem);
}
.panel-elm {
  border: 1px solid #cbd5e0;
  width: 160px;
  height: 40px;
  color: #319795;
}
.panel-elm p {
  text-align: center;
  font-weight: bold;
  font-size: 17px;
  letter-spacing: 0.84px;
}
.panel-1 {
  border-radius: 12px 0px 0px 12px;
}
.panel-3 {
  border-radius: 0px 12px 12px 0px;
}
.selected {
  background: #81e6d9;
  color: white;
}
</style>